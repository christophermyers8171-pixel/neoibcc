---
title: Cardiac Section Architecture (planning doc)
description: Internal planning document for the cardiology cluster. Not published.
draft: true
---

# NICU IBCC — Cardiology Section

*Status: architecture draft v0.1 · 2026-05-11*

---

## Section scope

Neonatal cardiovascular physiology, hemodynamic assessment, and the cardiovascular phenotypes encountered in the NICU. Not a substitute for pediatric cardiology resources — deep CHD lesion-by-lesion management belongs elsewhere and is cross-linked, not duplicated. The cluster's center of gravity is **neonatal hemodynamics and acquired cardiovascular dysfunction**, with CHD content limited to NICU-facing decisions (recognition, ductal-dependent stabilization, post-op management).

The reader this section is built for: a fellow or attending at the bedside trying to figure out whether a 25-weeker on epinephrine actually needs more pressor or more volume or a different pressor or none of the above. Bedside utility, opinionated, evidence-anchored.

---

## Chapter list

### Concept chapters (physiology backbone)

**1. Neonatal Hemodynamics Fundamentals** — *priority: near-term, write 1st*
The mental model. Transitional circulation, CO determinants in the immature heart, BP-vs-flow disconnect, oxygen delivery, end-organ perfusion markers, hemodynamic phenotyping framework. Everything else in the cluster cross-links back to this.

**2. Pulmonary Vascular Biology in the Neonate** — *priority: mid-term*
Why PVR doesn't fall normally. The postnatal PVR curve. NO pathway, prostacyclin pathway, endothelin pathway. Why pulmonary vasoreactivity matters. Foundation for PPHN, hsPDA, BPD-pulmonary hypertension chapters. Could fold into #1 in v1; separate it when content justifies.

### Modality chapters (the tools)

**3. TnECHO Basics: Image Acquisition** — *priority: near-term, write 2nd*
Standard views (PSLAX, PSSAX, A4C, A5C, subcostal, suprasternal), knobology calibrated for the neonate, normal anatomy, the "standard scan" sequence. Anchored on the McNamara 2024 ASE guidelines. Heavy use of image embeds.

**4. TnECHO Functional Assessment** — *priority: near-term, write 3rd*
Reading the scan. RV function (TAPSE, S', FAC, strain), LV function (FS, EF, MAPSE), cardiac output measurement (LVO, RVO, SVC flow), pulmonary hypertension assessment (TR jet, septal motion, RV pressure estimation). The Functional Assessment chapter is where the hemodynamic phenotyping framework gets operationalized.

**5. POCUS for the Neonatologist: Beyond the Heart** — *priority: mid-term*
Lung (B-lines, pleural sliding, effusions), brain (cranial ultrasound integrated), bladder. Less wheelhouse for you but increasingly part of the bedside hemodynamic assessment.

**6. NIRS in the NICU** — *priority: mid-term*
Cerebral and somatic NIRS. SafeBoosC II/III interpretation. The "what to do with the number" problem. Where it actually changes management vs. where it's decoration.

**7. Inhaled Nitric Oxide** — *priority: mid-term*
Physiology, dosing, weaning, the term/late preterm vs. preterm evidence gap. Indication creep critique.

**8. Prostaglandin E1 (Alprostadil)** — *priority: near-term, write early*
A small, high-value chapter. Indications, dose, side effects (apnea, hypotension, vasodilation), duration, what to watch for in transport. The kind of chapter a fellow or peds hospitalist who suddenly has a ductal-dependent baby will pull up at 3am.

**9. Inotropes & Vasopressors in the Neonate** — *priority: near-term, write 4th*
Dopamine, dobutamine, epinephrine, norepinephrine, vasopressin, milrinone. Neonatal-specific pharmacology (receptor maturation, why dopamine is weird in preterms). Phenotype-matched selection.

**10. Hydrocortisone for Refractory Hypotension** — *priority: mid-term*
Relative adrenal insufficiency framing, dosing, evidence base, when to use vs. when to keep titrating pressors.

### Procedure chapters

**11. UVC Placement and Management** — *priority: near-term*
Technique, tip position confirmation (which is contested), duration, complications, when to pull.

**12. UAC Placement and Management** — *priority: near-term*
High vs. low position controversy, complications, surveillance.

**13. Peripheral Arterial Line in the Neonate** — *priority: mid-term*
When to attempt, sites, complications.

### Approach-to-problem chapters

**14. Approach to the Hypotensive Preterm** — *priority: near-term, write 5th*
The flow chart you actually use. Confirm BP is real → assess for poor perfusion → identify phenotype (low CO vs. low SVR vs. obstructive) → match treatment to phenotype. Heavy cross-link to concept and modality chapters. This is where the BP-vs-flow philosophy operationalizes.

**15. Approach to the Cyanotic Newborn** — *priority: near-term*
Hyperoxia test, the differential (ductal-dependent CHD vs. PPHN vs. parenchymal lung disease vs. methemoglobinemia vs. polycythemia), initial workup, when to start PGE1 empirically.

**16. Approach to Acute Hemodynamic Deterioration in the NICU** — *priority: mid-term*
The "this baby is suddenly sicker" problem. Differential, rapid bedside assessment, common pitfalls (PTX, tamponade from line, sudden hsPDA opening, NEC).

**17. Approach to the Newborn with a Murmur** — *priority: low — common but textbook-covered*
Innocent vs. concerning, when to image, when to consult.

### Syndrome chapters

#### Transition & shunt physiology

**18. hsPDA: When (and Whether) to Treat** — *DRAFT EXISTS, write next: revise to template*
Already drafted. Will be the proof-of-template chapter.

**19. PPHN of the Newborn** — *priority: near-term, high-value*
Recognition, hyperoxia test interpretation, escalating management (oxygen, iNO, sildenafil, milrinone, ECMO), the term vs. preterm distinction. Where you'll likely have strong opinions.

**20. Ductal-Dependent CHD: Recognition & Initial Stabilization** — *priority: mid-term*
The NICU-facing slice of CHD. Recognition, PGE1, the "don't oxygenate" worry (overstated), when to transfer.

#### Shock & hemodynamic compromise

**21. Neonatal Septic Shock** — *priority: mid-term*
Cold vs. warm shock framework (acknowledging its limits), fluid resuscitation (cautious in preterms), pressor selection by phenotype, antibiotic timing. Crosses heavily with the ID cluster — decide which cluster "owns" it.

**22. HIE: The Hemodynamic Phenotype** — *priority: mid-term*
The cardiovascular dysfunction of HIE — myocardial dysfunction, pulmonary hypertension, the "double hit" during cooling. Distinct enough from the neuro management of HIE to warrant its own chapter (and gives a natural cross-link to the neuro cluster's HIE chapter).

**23. Neonatal Cardiogenic Shock** — *priority: long-term*
Rare. Myocarditis, severe LV dysfunction post-asphyxia, post-op LCOS. Could fold into post-cardiac-surgery chapter initially.

#### Post-cardiac surgical

**24. Post-Cardiac Surgery NICU Management** — *priority: long-term, fellowship-rotation-dependent*
LCOS, JET and other junctional rhythms, delayed sternal closure, chylothorax. Requires the cardiac NICU rotation experience to write authoritatively. Defer until then.

#### Other

**25. Neonatal Arrhythmias** — *priority: mid-term*
SVT (the most common one you actually manage), complete heart block (often maternal SSA/SSB), neonatal AF (rare), long QT recognition. Adenosine dosing, when to cardiovert.

**26. Neonatal Hypertension** — *priority: low*
Rare but real. Renovascular (UAC-associated), BPD-associated, endocrine. Diagnosis and initial management.

---

## Out of scope — cross-link only

These exist in pediatric cardiology resources and shouldn't be duplicated:

- Detailed lesion-specific CHD management (HLHS staging, single-ventricle pathway, TGA repair decisions)
- Cardiac catheterization techniques
- Surgical procedure decision-making
- Pediatric ICU post-op management beyond initial NICU stabilization
- Advanced electrophysiology beyond basic recognition

Suggested cross-links: AHA neonatal cardiology resources, Park's textbook, hospital pediatric cardiology consult service, and ideally a curated short list of FOAM resources in pediatric cardiology.

---

## Suggested write order

The dependency chain is concept → modality → approach → syndrome. But mechanical sequencing is wrong because nothing forces you to finish the concept chapter before drafting a syndrome chapter that depends on it — you'll iterate.

A realistic build order:

1. **Neonatal Hemodynamics Fundamentals** (concept) — sets the mental model and the chapter's organizing logic
2. **TnECHO Basics** (modality) — the tool that the rest of the cluster depends on
3. **TnECHO Functional Assessment** (modality) — operationalizes the phenotyping framework
4. **Inotropes & Vasopressors in the Neonate** (modality) — completes the modality triad
5. **Approach to the Hypotensive Preterm** (approach) — first chapter that uses everything above
6. **Revise hsPDA** to inherit from concept + modality (less to carry once the cluster scaffolding exists)
7. **PPHN of the Newborn** (syndrome) — pairs naturally with hsPDA
8. **Prostaglandin E1** + **Approach to the Cyanotic Newborn** (modality + approach pair)
9. **HIE: Hemodynamic Phenotype** (syndrome) — cross-bridges to neuro cluster

That's nine chapters. Realistic over the first 9–12 months of fellowship if you batch the modality work during cardiology/hemodynamics-relevant rotations. The remainder fills in over years 2–3.

Pre-fellowship target (the ~7-week beachhead): refine hsPDA + draft Hemodynamics Fundamentals + start TnECHO Basics outline. That's a real cluster foothold before July without overpromising.

---

## Open questions to decide before writing

1. **How much CHD?** Recommendation above is "NICU-facing only, cross-link the rest." Worth confirming.
2. **Does Septic Shock live in Cardio or ID?** Pick one and cross-link from the other.
3. **PPHN — its own chapter or folded into "Approach to the Cyanotic Newborn"?** Recommend its own chapter; cyanotic-newborn approach links to it.
4. **Cooling/HIE — is the hemodynamic phenotype really separable from the neuro management?** Recommend yes (you'd want hemodynamic specifics centralized), but it's a real call.
5. **Lung POCUS — Cardio cluster or Pulmonary cluster?** Recommend Pulmonary; cross-link.
