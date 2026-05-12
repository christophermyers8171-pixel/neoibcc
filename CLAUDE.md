# NeoIBCC

A free, opinionated, IBCC-style web resource for neonatal critical care. Modeled on Josh Farkas's Internet Book of Critical Care ([emcrit.org/ibcc](https://emcrit.org/ibcc)) but for the NICU. Center of gravity: **neonatal hemodynamics and acquired cardiovascular dysfunction**.

Target launch: June 2026.

## Stack

- **Quartz v4** static site generator (Obsidian-flavored markdown → static HTML)
- **GitHub** public repo: [christophermyers8171-pixel/neoibcc](https://github.com/christophermyers8171-pixel/neoibcc)
- **Cloudflare Workers + Static Assets** hosting — auto-builds on push to `v4`
- **Production branch:** `v4` (NOT `main`). This keeps the Quartz upgrade path clean: `git pull upstream v4` pulls framework updates from `jackyzha0/quartz`.

**Live URL:** https://neoibcc.christopher-myers8171.workers.dev/

## Daily workflow

### Author
Drafts vault lives outside the repo at `~/Desktop/NeoIBCC-Drafts/`. Open it as an Obsidian vault. Edit chapters there. The drafts vault is not in git — local writing space only.

When a chapter is ready to publish, copy it to the repo:
```bash
cp ~/Desktop/NeoIBCC-Drafts/cardiac/<chapter>.md ~/Desktop/dev/neoibcc/content/cardiac/<chapter>.md
```

### Publish
```bash
cd ~/Desktop/dev/neoibcc
git add . && git commit -m "..." && git push
```
~2 min later it's live. Cloudflare auto-builds on push.

### Preview locally
```bash
cd ~/Desktop/dev/neoibcc
npx quartz build --serve   # http://localhost:8080
```

### Pull Quartz framework updates
```bash
git pull upstream v4
```

## File organization

```
neoibcc/
├── content/                    # everything Quartz publishes
│   ├── index.md                # homepage
│   ├── cardiac/                # cardiology section
│   │   ├── index.md            # section TOC
│   │   └── <chapter>.md        # 26 chapter pages
│   └── private/                # NOT published (Quartz ignorePattern)
│       └── cardiac-section-architecture.md   # planning doc
├── quartz.config.ts            # site config (pageTitle, baseUrl, ignorePatterns)
├── quartz.layout.ts            # layout components (Explorer set to open by default)
├── wrangler.jsonc              # Cloudflare Workers config
└── CLAUDE.md                   # this file
```

`content/private/` is published-ignored but git-tracked. Use it for planning docs, internal notes, anything that shouldn't be on the live site but should be preserved with the project.

## Chapter conventions

### Five chapter types
| Type | Question it answers | Examples |
| --- | --- | --- |
| **Concept** | "What is this and why does it matter?" | Hemodynamics fundamentals |
| **Modality** | "How do I use this tool / drug?" | TnECHO, iNO, dopamine |
| **Procedure** | "How do I do this technique?" | UVC, UAC |
| **Approach** | "Patient has X — what now?" | Approach to hypotensive preterm |
| **Syndrome** | "What is this disease and how do I manage it?" | hsPDA, PPHN |

Templates for each type live in `~/Desktop/NeoIBCC-Drafts/zTemplates/`.

### Front-matter
```yaml
---
title: Human-readable chapter title
description: One sentence — used in search and link previews
tags:
  - <section>      # e.g., cardiac, respiratory, neuro
  - <type>         # concept | modality | procedure | approach | syndrome
---
```

### Wikilinks
Quartz uses Obsidian-style `[[link]]` syntax with shortest-path resolution. `[[pphn]]` resolves to `cardiac/pphn.md` from anywhere. Use `[[slug|Display Text]]` for renamed links.

### Callouts (Obsidian-style)
```markdown
> [!warning] Pitfall
> Content here.
```
Types: `note`, `info`, `tip`, `warning`, `danger`, `example`, `question`, `quote`.

## Architecture foot-guns — do NOT

- **Do not** reintroduce a symlink-based two-vault architecture pointing into a private Obsidian vault. Tried it, abandoned it: git won't push through a symlink and Cloudflare's build server can't follow one. The drafts vault on Desktop with copy-on-publish is the deliberate replacement.
- **Do not** rename the production branch to `main`. Cloudflare is configured to deploy from `v4`. Changing the branch name breaks the Quartz upgrade path (`git pull upstream v4`).
- **Do not** edit `quartz.config.ts` `ignorePatterns` to remove `private/`. The `content/private/` folder relies on this to stay off the live site.
- **Do not** commit the `~/Desktop/NeoIBCC-Drafts/` folder. It is intentionally outside the repo as a writing-only space.

## Known gotchas

### Cloudflare deploy command
The deploy command **must** be `npx wrangler deploy --assets=./public` — not `wrangler versions upload`. The `versions upload` command uploads but does not promote to production, leaving new pushes stuck as previews. Both production and non-production branch deploy commands need this.

If a push appears to build successfully but the live site doesn't update, this is the first thing to check. The setting lives in: Cloudflare dashboard → project → Settings → Build → Build configuration.

### Build cache
Cloudflare's build cache occasionally serves stale node_modules. If a build fails for no obvious reason, clear the build cache (Settings → Build → Build cache → Clear).

### Date warnings during local build
`Warning: content/X.md isn't yet tracked by git` is harmless and disappears after the file is committed. Quartz uses git history for last-modified dates.

## Useful commands

```bash
# Start dev server
cd ~/Desktop/dev/neoibcc && npx quartz build --serve

# Production build (sanity check before push)
npx quartz build

# Pull Quartz framework updates from upstream
git pull upstream v4

# View deployment status (requires gh CLI)
gh repo view christophermyers8171-pixel/neoibcc --web
```

## References

- Quartz docs: https://quartz.jzhao.xyz/
- Cardiology section planning doc: `content/private/cardiac-section-architecture.md`
