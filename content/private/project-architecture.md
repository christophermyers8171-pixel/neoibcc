---
title: NeoIBCC — Full Project Architecture
description: Internal planning document — scope and chapter list for all 12 clusters. Not published.
draft: true
---

# NeoIBCC — Full Project Architecture

*Status: architecture draft v0.1 · 2026-05-11 · Companion to cardiac-section-architecture.md*

---

## Project-level decisions (apply to all clusters)

**Chapter types** (carry through every cluster):
- **Concept** — physiology / mental model. Pathophys-forward.
- **Modality** — interventions and tools. Physiology up front (it organizes the chapter).
- **Procedure** — technique-focused.
- **Approach-to-problem** — decision-tree shaped, links to syndrome chapters.
- **Syndrome** — disease-specific. Rapid reference → diagnosis → causes → treatment → deep pathophys at end.

**Out-of-scope rule:** if a topic is well-covered by an existing resource (NeoReviews, Cloherty, MGH Manual, AAP) and you don't have an opinionated or operationally distinct take, cross-link rather than duplicate. The site adds value where there's a gap or where opinion matters.

**Cross-cutting "Guide to NICU Bedside Care"** — single meta-chapter (Farkas's "Guide to supportive care" analog). Covers universals so individual chapters don't repeat: temperature regulation, line care, monitoring basics, developmental care, pain/sedation framework, feeding support basics, family-centered care. Cross-linked everywhere.

---

## Cluster 1: Cardiology & Hemodynamics

*Covered in detail in cardiac-section-architecture.md. ~26 chapters across concept (2), modality (8), procedure (3), approach (4), syndrome (9). Pre-fellowship beachhead: refine hsPDA + draft Hemodynamics Fundamentals + start TnECHO Basics.*

---

## Cluster 2: Pulmonary & Respiratory

### Scope

Neonatal pulmonary disease, respiratory support, and ventilator management. Center of gravity is the preterm lung. CDH lives here (with cardio cross-link for the PPHN component). Airway anomalies cross-link to ENT/peds airway resources rather than duplicate.

Reader: bedside clinician trying to figure out whether a 25-weeker not extubating is BPD evolution, residual surfactant deficiency, hsPDA, or just under-sedated.

### Concept chapters

1. **Pulmonary Mechanics in the Premature Lung** *(near-term, high-priority)* — Compliance, resistance, time constants, why preemies are different. Foundation for ventilator chapters.
2. **Surfactant Biology** *(mid-term)* — Composition, surface tension, the type II pneumocyte, what surfactant deficiency actually does to pressure-volume curves. Sets up RDS and surfactant administration chapters.
3. **Lung Development & Alveolarization** *(long-term)* — Canalicular, saccular, alveolar stages. Why <26 wk lungs are different from 32 wk lungs. Foundation for BPD chapter.
4. **Gas Exchange in the Neonate** *(mid-term)* — V/Q, shunt, diffusion limitation, why the neonate's curves are different. Sets up oxygen targeting.

### Modality chapters

5. **Non-Invasive Ventilation: CPAP, NIPPV, HFNC** *(near-term)* — Indications, settings, escalation thresholds. The "is this enough?" question.
6. **Conventional Mechanical Ventilation in the Neonate** *(near-term, high-priority)* — Modes, volume-targeted vs pressure-limited, settings, weaning. Probably your single most-read chapter once published.
7. **High-Frequency Oscillatory Ventilation (HFOV)** *(mid-term)* — Indications, settings (MAP, amplitude, frequency), troubleshooting. Opinionated on rescue vs first-line.
8. **High-Frequency Jet Ventilation (HFJV)** *(mid-term)* — Indications (especially air leak), settings, when to choose over HFOV.
9. **Surfactant Administration** *(near-term)* — INSURE, LISA/MIST, dose, repeat dosing criteria, prophylactic vs rescue.
10. **Inhaled Nitric Oxide** — *Lives in Cardio cluster; cross-link from here.*
11. **Pulmonary Mechanics Monitoring** *(mid-term)* — Graphics interpretation, loops, real-world bedside use. Often under-taught.
12. **Postnatal Steroids in BPD** *(mid-term)* — Dexamethasone, hydrocortisone, the DART regimen. Where opinion strongly matters.
13. **Diuretics for BPD** *(mid-term)* — Furosemide, thiazide/spironolactone. Evidence-thin but practice-heavy area.

### Procedure chapters

14. **Neonatal Intubation** *(near-term)* — Technique, premedication (atropine, fentanyl, vecuronium), tube selection, depth, confirmation. Difficult airway pathway.
15. **LISA/MIST Technique** *(mid-term)* — The procedure itself, separate from the modality chapter on surfactant.
16. **Extubation Assessment** *(near-term)* — When to attempt, predictors, post-extubation support choice.

### Approach-to-problem chapters

17. **Approach to the Desatting Newborn** *(near-term)* — The differential, the rapid bedside assessment, when to escalate. *Cross-cluster with Cardio.*
18. **Approach to Persistent Oxygen Requirement** *(near-term)* — The 28-day, 36-week framework, the differential beyond "BPD," workup pathway.
19. **Approach to Extubation Failure** *(mid-term)* — Why this baby failed, what changes for the next attempt.
20. **Approach to Acute Respiratory Deterioration** *(mid-term)* — The "this baby is suddenly sicker" differential. PTX, tube malposition, mucus plug, blood, sudden PDA, sepsis.

### Syndrome chapters

21. **Respiratory Distress Syndrome (RDS)** *(near-term, high-priority)* — The classic. Pathophys, presentation, surfactant decision, support strategy.
22. **Bronchopulmonary Dysplasia (BPD): Recognition & Definition** *(near-term)* — The Jensen 2019 definition, severity grading, why definitions matter.
23. **BPD: Trajectory & Management** *(near-term)* — Where your research interest aligns with the writing. Trajectory phenotypes, established vs evolving, when to escalate care. Could be flagship chapter.
24. **BPD-Associated Pulmonary Hypertension** *(mid-term)* — Screening, recognition, management. Cross-link to Cardio.
25. **Transient Tachypnea of the Newborn (TTN)** *(near-term)* — Recognition, when to image, when it's not TTN.
26. **Meconium Aspiration Syndrome (MAS)** *(mid-term)* — Severity stratification, surfactant role, PPHN overlap, ECMO threshold.
27. **Air Leak Syndromes: Pneumothorax, PIE, Pneumomediastinum** *(near-term)* — Recognition, transillumination, drainage decisions, HFJV role in PIE.
28. **Pulmonary Hemorrhage** *(mid-term)* — Recognition, management, the PDA association.
29. **Congenital Diaphragmatic Hernia (CDH)** *(mid-term)* — Pre-op stabilization, PPHN management, surgical timing decisions. Heavy cross-link with Cardio.
30. **Pulmonary Hypoplasia (non-CDH)** *(long-term)* — Causes (oligohydramnios, mass effect), recognition, management.
31. **Congenital Lung Lesions: CPAM, Sequestration, CLE** *(long-term)* — NICU-facing recognition and stabilization. Cross-link to surgical.
32. **Chronic Lung Disease in the Post-Discharge Window** *(long-term)* — Tracheostomy decision, home oxygen, prognosis conversations.

### Cross-cluster decisions

- **Where does iNO live?** Recommendation: Cardio (it's primarily a pulmonary-vascular intervention). Cross-link from Pulmonary.
- **Where does PPHN live?** Recommendation: Cardio. Cross-link from Pulmonary (especially MAS, CDH).
- **Where does CDH live?** Recommendation: Pulmonary (lung-centric primary diagnosis). Cross-link from Cardio for PPHN management.
- **Where does HIE-related respiratory dysfunction live?** Brief mention here, primary chapter in Neuro.

### Suggested write order (Pulmonary)

1. RDS (foundational syndrome, often co-written with surfactant modality)
2. Surfactant Administration
3. Conventional Mechanical Ventilation
4. Pulmonary Mechanics in the Premature Lung
5. Non-Invasive Ventilation
6. BPD: Recognition & Definition
7. BPD: Trajectory & Management (your research-aligned flagship)
8. Approach to the Desatting Newborn
9. Approach to Persistent Oxygen Requirement

---

## Cluster 3: Neurology

### Scope

Neonatal neurologic disease, neuro-monitoring, and bedside neurology in the NICU. Center of gravity is HIE, IVH, and seizures. Long-term neurodevelopmental follow-up is out of scope. Detailed peds neurology / neurosurgery cross-link out.

Reader: bedside clinician trying to figure out whether a movement was a seizure, whether a head ultrasound finding requires action, or whether a HIE infant is on the right cooling and hemodynamic trajectory.

### Concept chapters

1. **Cerebral Autoregulation in the Preterm** *(near-term, high-priority)* — The pressure-passive cerebral circulation, the lower limit of autoregulation, why BP matters here. Foundation for IVH and HIE chapters.
2. **Neonatal Brain Development** *(mid-term)* — Germinal matrix, periventricular white matter, vulnerability windows by gestational age. Foundation for IVH and PVL.
3. **Cerebral Blood Flow & Oxygen Consumption in the Neonate** *(mid-term)* — Quantitative neonatal cerebral physiology. Foundation for NIRS interpretation.
4. **Mechanisms of Neonatal Brain Injury** *(mid-term)* — Excitotoxicity, oxidative stress, the reperfusion cascade. Why cooling works. Foundation for HIE management.

### Modality chapters

5. **Therapeutic Hypothermia (Cooling)** *(near-term, high-priority)* — Criteria, initiation, monitoring during cooling, rewarming, the "cool late preterms?" question, complications.
6. **Cranial Ultrasound: Acquisition & Interpretation** *(near-term)* — Standard views, normal anatomy, grading IVH, PVL recognition, ventricular size. Heavy use of image embeds.
7. **aEEG / Conventional EEG in the Neonate** *(near-term)* — When to use which, interpretation basics, burst suppression, seizure detection sensitivity.
8. **Neonatal MRI: When and How to Interpret** *(mid-term)* — Indications, DWI/ADC in HIE, scoring systems, timing post-injury.
9. **NIRS for Cerebral Oximetry** — *Cross-cluster; could live here or Cardio. Recommend: Cardio for general NIRS, brief Neuro-specific section here.*
10. **Anticonvulsants in the Neonate** *(near-term)* — Phenobarbital, fosphenytoin, levetiracetam, midazolam. Dosing, evidence base, the levetiracetam vs phenobarbital question.

### Procedure chapters

11. **Lumbar Puncture in the Neonate** *(near-term)* — Technique, timing, contraindications, interpretation. *Cross-cluster with ID.*

### Approach-to-problem chapters

12. **Approach to Neonatal Seizures** *(near-term, high-priority)* — Recognition (subtle vs clonic vs tonic), differential, workup pathway, initial treatment.
13. **Approach to the Floppy Infant** *(mid-term)* — Central vs peripheral, the differential, workup. Cross-link to metabolic and genetics.
14. **Approach to Abnormal Cranial Ultrasound Findings** *(near-term)* — IVH grades, what to do, ventricular dilation tracking, when neurosurgery needs to be involved.
15. **Approach to Suspected Neonatal Stroke** *(mid-term)* — Presentation, imaging timing, workup, management.
16. **Approach to the Apparent HIE That Isn't** *(mid-term)* — Mimics: metabolic, infection, stroke, IEM. When to think differently.

### Syndrome chapters

17. **Hypoxic-Ischemic Encephalopathy (HIE): Recognition & Initial Management** *(near-term, high-priority)* — Sarnat staging, cooling decision, the 6-hour window, who not to cool.
18. **HIE: Hemodynamic & Multi-Organ Phenotype** — *Cross-cluster with Cardio. Recommend home: Neuro for the neuro-centric chapter, Cardio for the hemodynamic phenotype, both cross-linked.*
19. **Intraventricular Hemorrhage (IVH)** *(near-term)* — Pathogenesis, grading, prevention, progression, post-hemorrhagic ventricular dilation.
20. **Periventricular Leukomalacia (PVL)** *(mid-term)* — Cystic vs non-cystic, recognition, prognosis conversation.
21. **Neonatal Seizures** *(near-term)* — Causes by GA and timing, EEG-confirmed vs clinical, treatment escalation, when to taper.
22. **Neonatal Stroke** *(mid-term)* — Arterial ischemic, hemorrhagic, venous sinus thrombosis. Workup and management.
23. **Birth Trauma: Brachial Plexus, Cephalohematoma, Subgaleal, Skull Fracture** *(mid-term)* — Recognition, severity, management, follow-up.
24. **Hydrocephalus in the Neonate** *(mid-term)* — Causes, recognition, ventricular tap vs reservoir vs shunt timing.
25. **Neural Tube Defects: Initial NICU Management** *(long-term)* — Pre-op care, post-op management, hydrocephalus surveillance.
26. **CNS Infection: Meningitis & Encephalitis** — *Cross-cluster with ID. Recommend home: ID.*

### Cross-cluster decisions

- **HIE: where's the home?** Recommend: split. Neuro owns the neurologic chapter (Sarnat, EEG, MRI, cooling decision). Cardio owns the hemodynamic phenotype chapter. Both cross-link.
- **Neonatal seizures: where's the home?** Recommend: Neuro (anticonvulsants, EEG, syndromic causes). Metabolic and ID cross-link from their causes.
- **Inborn errors with neuro presentation:** approach chapter here cross-linking to detailed IEM chapters in Endocrine/Metabolic.

### Suggested write order (Neurology)

1. HIE: Recognition & Initial Management (high-yield, fellowship-relevant fast)
2. Therapeutic Hypothermia
3. Cranial Ultrasound: Acquisition & Interpretation
4. Approach to Neonatal Seizures
5. Anticonvulsants in the Neonate
6. IVH (syndrome)
7. Cerebral Autoregulation in the Preterm (concept, anchors the cluster)
8. aEEG / Conventional EEG in the Neonate
9. Approach to Abnormal Cranial Ultrasound Findings

---

## Cluster 4: Infectious Disease

### Scope

Neonatal infection — recognition, workup, empiric antimicrobials, organism-specific management. Vertical transmission (TORCH and HIV/Hep B). Stewardship is woven through rather than its own chapter. Adult ID and detailed virology are cross-link.

Reader: bedside clinician trying to figure out whether a 25-weeker with new apnea needs a full sepsis workup, whether a positive blood culture is real, or whether to broaden coverage.

### Concept chapters

1. **The Neonatal Immune System** *(mid-term)* — Why neonates (especially preterms) are different. Neutrophil function, complement, antibody, gut barrier. Foundation for everything.
2. **Vertical Transmission: Maternal-Fetal Infection Dynamics** *(mid-term)* — GBS colonization → EOS, chorioamnionitis, the modified intrapartum risk frameworks (Kaiser calculator).

### Modality chapters

3. **Empiric Antimicrobials in the Neonate** *(near-term, high-priority)* — Ampicillin + gentamicin vs alternatives, when to broaden, when to narrow. The "default cocktail" chapter.
4. **Aminoglycoside Dosing & Monitoring** *(near-term)* — Extended-interval dosing, levels, renal considerations.
5. **Vancomycin in the Neonate** *(near-term)* — Dosing, AUC vs trough, when to use, when not to.
6. **Antifungal Selection** *(mid-term)* — Fluconazole prophylaxis (and the Kaufman critique you've already engaged with), amphotericin, micafungin. Indications and dosing.
7. **Antivirals in the Neonate** *(mid-term)* — Acyclovir for HSV, ganciclovir/valganciclovir for CMV. Dosing and monitoring.
8. **IVIG in Neonatal Sepsis** *(long-term)* — The evidence (mostly negative for prevention/treatment), narrow indications.

### Procedure chapters

9. **Lumbar Puncture in Sepsis Workup** — *Lives in Neuro cluster; cross-link from here.*

### Approach-to-problem chapters

10. **Approach to Suspected Early-Onset Sepsis** *(near-term, high-priority)* — The Kaiser calculator, the categorical risk framework, when to treat. Heavily opinionated territory.
11. **Approach to Suspected Late-Onset Sepsis** *(near-term)* — The differential by site (CLABSI vs pneumonia vs UTI vs meningitis), workup tiers, empiric coverage.
12. **Approach to Fever in the Term Newborn** *(mid-term)* — Outpatient and ED framework, the AAP guideline.
13. **Approach to Persistent Positive Blood Cultures** *(mid-term)* — Source-finding workflow, contaminant vs real, when to remove lines.
14. **Approach to the Infant of a Mother with HIV / Hep B / Syphilis / GBS / HSV / Maternal Fever** *(mid-term)* — Each gets a section or its own short chapter.

### Syndrome chapters

15. **Early-Onset Sepsis (EOS)** *(near-term)* — GBS, E. coli, Listeria. Presentation, workup, treatment duration.
16. **Late-Onset Sepsis (LOS)** *(near-term)* — CoNS, S. aureus, gram-negatives, fungi. Source-driven differential.
17. **Neonatal Meningitis** *(mid-term)* — Workup (LP interpretation in neonate), treatment duration, complications.
18. **Catheter-Related Bloodstream Infection (CLABSI / CoNS Bacteremia)** *(near-term)* — When to remove the line, when not to, antibiotic course, the CoNS "is it real" problem you've thought about.
19. **Neonatal Pneumonia** *(mid-term)* — Congenital vs ventilator-associated, recognition, treatment.
20. **Necrotizing Fasciitis & Severe Skin/Soft Tissue Infection** *(long-term)* — Rare, but recognition matters.
21. **Omphalitis** *(mid-term)* — Recognition, severity, antibiotic choice.
22. **Conjunctivitis: Chemical vs GC vs Chlamydia vs HSV** *(mid-term)* — Timing-based differential.
23. **Congenital HSV** *(near-term)* — Categories (SEM, CNS, disseminated), workup, treatment.
24. **Congenital CMV** *(near-term)* — Screening, hearing loss, when to treat with valganciclovir.
25. **Congenital Syphilis** *(mid-term)* — Workup pathway by maternal status, treatment.
26. **Congenital Toxoplasmosis** *(long-term)* — Recognition, treatment.
27. **Congenital Rubella, Varicella, Zika, Parvovirus** *(long-term)* — Brief recognition-focused chapters.
28. **Neonatal HIV Exposure & Management** *(mid-term)* — Antiretroviral prophylaxis, testing schedule.
29. **Neonatal Tuberculosis & Maternal TB Exposure** *(long-term)* — Workup and prophylaxis.
30. **Neonatal Septic Shock** — *Cross-cluster with Cardio. Recommend home: ID, with strong hemodynamic cross-link.*
31. **Necrotizing Enterocolitis** — *Cross-cluster with GI. Recommend home: GI.*

### Cross-cluster decisions

- **Septic shock home:** ID (with full hemodynamic management cross-linked to Cardio's hypotension framework and pressor selection).
- **CNS infections home:** ID (with neuro-imaging cross-linked to Neuro).
- **UTI home:** Renal (cross-link from ID).
- **NEC home:** GI (cross-link from ID).

### Suggested write order (ID)

1. Approach to Suspected Early-Onset Sepsis (most-read chapter likely)
2. Empiric Antimicrobials in the Neonate
3. Early-Onset Sepsis (syndrome)
4. Approach to Suspected Late-Onset Sepsis
5. Late-Onset Sepsis (syndrome)
6. CLABSI / CoNS Bacteremia (your existing case experience here)
7. Vancomycin in the Neonate
8. Congenital HSV
9. Congenital CMV

---

## Cluster 5: Gastrointestinal & Nutrition

### Scope

Neonatal GI disease, feeding management, nutrition (enteral and parenteral), and the GI side of NEC. Cholestasis lives here. Surgical GI conditions are cross-link to the surgical cluster.

Reader: bedside clinician trying to decide whether to hold feeds on an infant with bilious aspirates, when to start fortification, or whether a non-specific abdominal X-ray is NEC.

### Concept chapters

1. **Enteral Feeding Physiology in the Preterm** *(mid-term)* — Gut motility, digestive enzyme maturation, the rationale for trophic feeds.
2. **Gut Maturation & The Microbiome in the Preterm** *(mid-term)* — Postnatal colonization, probiotics evidence (the moving target), why this matters for NEC.
3. **Parenteral Nutrition: Composition & Physiology** *(mid-term)* — Macros, micros, why neonatal PN is different.
4. **Growth in the Preterm: Targets & Trajectories** *(near-term)* — Fenton, Olsen, postnatal growth restriction, the "catch-up" vs "tracking" question.

### Modality chapters

5. **Enteral Feeding Protocols** *(near-term, high-priority)* — Initiation, advancement, fortification timing, donor milk vs formula decision points. Heavily institution-dependent — your opinion matters.
6. **Parenteral Nutrition Prescribing** *(near-term)* — Day-by-day buildup, soybean vs SMOF vs Omegaven, electrolyte titration, when to wean.
7. **Trophic Feeds & Minimal Enteral Nutrition** *(mid-term)* — Evidence, what counts, when to push past trophic.
8. **Probiotics in the NICU** *(mid-term)* — Strain-specific evidence, institutional adoption, the live-organism risk question.
9. **Pharmacologic Reflux Management** *(mid-term)* — H2 blockers, PPIs, prokinetics. Heavily opinionated — your "stop doing this" chapter.

### Procedure chapters

10. **NG / OG Tube Placement & Confirmation** *(near-term)* — Technique, confirmation methods, complications.

### Approach-to-problem chapters

11. **Approach to Feeding Intolerance** *(near-term, high-priority)* — Differential, when to hold, when to image, when it's not NEC.
12. **Approach to Abdominal Distention** *(near-term)* — Differential by GA and timing, imaging decisions.
13. **Approach to Bloody Stools** *(near-term)* — NEC vs swallowed blood vs allergic colitis vs anal fissure. Workup.
14. **Approach to Suspected NEC** *(near-term, high-priority)* — The rapid bedside workup, when to call surgery, when to make NPO. Heavy cross-link to the NEC syndrome chapter.
15. **Approach to Direct Hyperbilirubinemia / Cholestasis** *(near-term)* — Workup pathway, when biliary atresia is on the differential, urgency.
16. **Approach to Bilious Emesis** *(mid-term)* — The "malrotation until proven otherwise" workup.

### Syndrome chapters

17. **Necrotizing Enterocolitis (NEC): Recognition & Medical Management** *(near-term, flagship)* — Bell staging, imaging, antibiotic course, when to repeat XR. Heavy opinion territory.
18. **NEC: Surgical Management & When to Operate** *(mid-term)* — Indications, peritoneal drain vs primary laparotomy, post-op course.
19. **Spontaneous Intestinal Perforation (SIP)** *(near-term)* — Distinguishing from NEC, risk factors (early indomethacin/steroid), management.
20. **Gastroesophageal Reflux Disease (GERD) — and What Isn't** *(mid-term)* — Physiologic vs pathologic, the over-diagnosis problem.
21. **Cholestasis in the NICU** *(mid-term)* — TPN-associated, biliary atresia, infection, metabolic. Workup and management.
22. **Short Bowel Syndrome** *(long-term)* — Post-NEC, post-resection. Long-term management overview.
23. **Gastroschisis: NICU Management** *(mid-term)* — Pre-op, post-op course, feeding initiation. Cross-link surgical.
24. **Omphalocele: NICU Management** *(mid-term)* — Associated anomalies, staged closure decisions. Cross-link surgical.
25. **Esophageal Atresia / Tracheoesophageal Fistula: NICU Management** *(mid-term)* — Pre-op, post-op feeding, complications.
26. **Intestinal Atresia (Duodenal, Jejunal, Ileal)** *(mid-term)* — Recognition by level, pre/post-op management.
27. **Hirschsprung's Disease** *(mid-term)* — Recognition (delayed meconium), workup, initial management.
28. **Meconium Plug & Meconium Ileus** *(mid-term)* — Distinguishing, CF screening implication.
29. **Imperforate Anus** *(long-term)* — Initial management, associated anomalies (VACTERL).
30. **Pyloric Stenosis** *(long-term)* — Often post-discharge; brief chapter for the NICU-presenting case.
31. **Lactose Intolerance & Cow's Milk Protein Allergy in the NICU** *(mid-term)* — Recognition, formula switching, when it's not allergy.

### Cross-cluster decisions

- **Cholestasis home:** GI (it's a hepatic problem first).
- **TPN-associated liver disease:** subsection of Cholestasis chapter.
- **Gastroschisis/omphalocele surgical technique:** Surgical cluster cross-link; this cluster handles NICU course.
- **CDH:** Pulmonary (lung-centric primary diagnosis).
- **NEC:** GI primary home; ID and Surgical cross-link.

### Suggested write order (GI / Nutrition)

1. NEC: Recognition & Medical Management (flagship, high-yield)
2. Approach to Suspected NEC
3. Enteral Feeding Protocols
4. Approach to Feeding Intolerance
5. Spontaneous Intestinal Perforation
6. Parenteral Nutrition Prescribing
7. Approach to Bloody Stools
8. Pharmacologic Reflux Management (your "stop doing this" chapter)
9. Cholestasis in the NICU

---

## Cluster 6: Hematology

### Scope

Neonatal blood disorders, transfusion medicine, coagulation, and thrombosis. Heavy emphasis on the differences from adult hematology (fetal hgb, developmental hemostasis, vit K dependence).

Reader: bedside clinician trying to decide whether to transfuse a stable 27-weeker with hct 27, whether a thrombocytopenia is consumption or production, or whether to give vitamin K vs FFP for a coagulopathic premie.

### Concept chapters

1. **Neonatal Hematopoiesis & Developmental Hemostasis** *(mid-term)* — Why neonatal labs (PT/PTT, platelet count) look different. Coagulation factor maturation. Foundation for everything.
2. **Fetal vs Adult Hemoglobin: Oxygen Carrying & Transfusion Implications** *(mid-term)* — Why the oxygen-binding curve shifts matter.
3. **Vitamin K & Neonatal Coagulation** *(near-term)* — Why VKDB happens, IM vs oral, the "anti-vax refusal" framing.

### Modality chapters

4. **Blood Product Selection in the Neonate** *(near-term, high-priority)* — PRBC (irradiated, CMV-safe, leukoreduced), platelets, FFP, cryoprecipitate. When to use each.
5. **Transfusion Thresholds: PRBC** *(near-term)* — TOP, ETTNO, the converged guidelines. Opinion territory.
6. **Transfusion Thresholds: Platelets** *(near-term)* — PlaNeT-2 and the field's shift. You have strong opinions here; chapter writes itself.
7. **Vitamin K Administration** *(mid-term)* — Dosing, indications beyond newborn prophylaxis.
8. **Erythropoietin / Darbepoetin in the NICU** *(mid-term)* — Indications, evidence, the renewed interest for neuroprotection.

### Procedure chapters

9. **Exchange Transfusion: Technique** *(mid-term)* — When to do, how to do, complications. Cross-link bilirubin.
10. **Partial Exchange for Polycythemia** *(mid-term)* — Indications (rare), technique.

### Approach-to-problem chapters

11. **Approach to Neonatal Anemia** *(near-term)* — Acute vs chronic, hemolytic vs hemorrhagic vs production failure, workup pathway.
12. **Approach to Neonatal Thrombocytopenia** *(near-term, high-priority)* — Timing-based differential (early vs late), the NAIT workup, when to transfuse.
13. **Approach to Neonatal Bleeding** *(near-term)* — Differential by site, coag workup interpretation, treatment choice.
14. **Approach to Polycythemia** *(mid-term)* — Symptomatic vs not, partial exchange decision.
15. **Approach to Hydrops Fetalis** *(mid-term)* — Immune vs non-immune, workup, initial management.

### Syndrome chapters

16. **Anemia of Prematurity** *(near-term)* — Pathogenesis, transfusion vs EPO, growth implications.
17. **Hemolytic Disease of the Newborn: ABO, Rh, Other** *(near-term)* — Recognition, severity stratification, exchange transfusion threshold.
18. **Vitamin K Deficiency Bleeding (VKDB)** *(mid-term)* — Classic, late, the parental-refusal scenario.
19. **Neonatal DIC** *(mid-term)* — Recognition, underlying causes, treatment.
20. **Neonatal Alloimmune Thrombocytopenia (NAIT)** *(mid-term)* — Recognition, workup, treatment, future-pregnancy counseling.
21. **Neonatal Thrombosis & Thromboembolism** *(mid-term)* — Catheter-associated, renal vein, sinus venous. Anticoagulation decisions.
22. **Polycythemia / Hyperviscosity** *(mid-term)* — Causes, symptoms, partial exchange decision.
23. **Congenital Bone Marrow Failure Syndromes (Recognition)** *(long-term)* — Diamond-Blackfan, Fanconi, etc. NICU-relevant presentation.

### Cross-cluster decisions

- **Hemolytic disease + bilirubin:** Heme owns hemolysis; Bilirubin owns the management. Heavy cross-link.
- **Renal vein thrombosis:** Heme owns the thrombosis chapter; Renal cross-links from RVT-as-AKI-cause.
- **Sinus venous thrombosis:** Heme owns; Neuro cross-links.

### Suggested write order (Heme)

1. Approach to Neonatal Thrombocytopenia
2. Transfusion Thresholds: Platelets (your PlaNeT-2 chapter)
3. Transfusion Thresholds: PRBC
4. Blood Product Selection in the Neonate
5. Approach to Neonatal Anemia
6. Anemia of Prematurity
7. Hemolytic Disease of the Newborn
8. Approach to Neonatal Bleeding
9. Developmental Hemostasis (concept anchor)

---

## Cluster 7: Renal, Fluids & Electrolytes

### Scope

Neonatal renal function, fluid management in the first week of life and beyond, electrolyte disorders, and congenital renal anomalies relevant to the NICU.

Reader: bedside clinician trying to figure out fluid management on day 3 of a 24-weeker, whether oliguria is concerning, or what to do about a sodium of 152.

### Concept chapters

1. **Renal Physiology in the Preterm** *(mid-term)* — GFR maturation, tubular function, why neonatal creatinine is misleading, the postnatal transition.
2. **Insensible Water Losses & Fluid Physiology in the First Week** *(near-term, high-priority)* — Why <26-weekers leak. Foundation for fluid prescribing.
3. **Sodium Homeostasis in the Neonate** *(mid-term)* — Postnatal sodium handling, why hyponatremia is so common.

### Modality chapters

4. **Fluid Prescribing in the First Week** *(near-term, high-priority)* — Starting volumes, adjustments by weight/sodium/output. Strong opinion territory.
5. **Fluid Prescribing After Transition** *(mid-term)* — Standard maintenance, when to adjust.
6. **Diuretics in the Neonate** — *Lives in Pulmonary cluster; cross-link from here.*
7. **Renal Replacement Therapy in the Neonate** *(long-term)* — Peritoneal dialysis, CRRT, when. Rare but high-stakes.

### Procedure chapters

8. **Suprapubic Bladder Aspiration** *(mid-term)* — Technique, when over catheterization.
9. **Bladder Catheterization in the Neonate** *(mid-term)* — Technique, indications.

### Approach-to-problem chapters

10. **Approach to AKI in the Neonate** *(near-term)* — KDIGO definitions in neonates (mod 2017), workup, treatment.
11. **Approach to Hyponatremia** *(near-term)* — By timing (early vs late), severity-based treatment.
12. **Approach to Hypernatremia** *(near-term)* — Dehydration vs sodium loading, correction rate.
13. **Approach to Hyperkalemia** *(near-term, high-priority)* — Non-oliguric (extreme preterm) vs oliguric, treatment escalation.
14. **Approach to Hypokalemia** *(mid-term)* — Causes, repletion.
15. **Approach to Hypocalcemia** — *Lives in Endocrine cluster; cross-link from here.*
16. **Approach to Oliguria** *(near-term)* — Differential, workup, when to intervene.
17. **Approach to the Antenatally-Detected Renal Anomaly** *(mid-term)* — Hydronephrosis, MCDK, etc. Postnatal workup pathway.

### Syndrome chapters

18. **Neonatal AKI** *(near-term)* — Etiologies by setting (HIE, sepsis, NSAIDs, RVT), management, RRT decision.
19. **Renal Vein Thrombosis** — *Lives in Heme cluster; cross-link.*
20. **Posterior Urethral Valves (NICU Management)** *(mid-term)* — Recognition, initial decompression, workup.
21. **Multicystic Dysplastic Kidney** *(long-term)* — Antenatal vs postnatal, surveillance.
22. **Bartter Syndrome (Antenatal)** *(long-term)* — Recognition, electrolyte management.
23. **UTI in the Neonate** — *Cross-cluster with ID. Recommend home: Renal.*
24. **Hypertension in the Neonate** *(mid-term)* — Renovascular (UAC-associated), BPD-associated, endocrine. Workup and initial management.

### Cross-cluster decisions

- **Fluid management:** Renal owns it (more than Endocrine or Cardio).
- **Diuretics:** Pulmonary owns the BPD-driven chapter; this cluster cross-links.
- **Hypocalcemia/hypoglycemia:** Endocrine owns.

### Suggested write order (Renal)

1. Fluid Prescribing in the First Week (universally relevant)
2. Insensible Water Losses & Fluid Physiology
3. Approach to Hyperkalemia
4. Approach to AKI in the Neonate
5. Approach to Hyponatremia
6. Neonatal AKI (syndrome)
7. Approach to Oliguria
8. Approach to Hypernatremia
9. Hypertension in the Neonate

---

## Cluster 8: Endocrine & Metabolic

### Scope

Glucose homeostasis (the dominant chunk), calcium/phosphorus, thyroid, adrenal, inborn errors of metabolism, and abnormal newborn screen workup.

Reader: bedside clinician trying to figure out whether to push past D12.5 in a persistently hypoglycemic infant, what an abnormal newborn screen result means, or whether an unexplained encephalopathy is metabolic.

### Concept chapters

1. **Neonatal Glucose Homeostasis** *(near-term, high-priority)* — Postnatal glucose transition, why the curves look how they look, regulatory hormones.
2. **Calcium & Phosphorus Metabolism in the Newborn** *(mid-term)* — Early vs late hypocalcemia, the PTH transition.
3. **Thyroid Function in the Newborn** *(mid-term)* — The TSH surge, the newborn screen, transient vs permanent disease.
4. **Adrenal Physiology in the Preterm** *(mid-term)* — Relative adrenal insufficiency, the postnatal cortisol curve.

### Modality chapters

5. **Glucose Infusion Rate (GIR) Management** *(near-term)* — Calculating, escalating, when to add fat/protein.
6. **Insulin in the Neonate** *(mid-term)* — Indications (mostly hyperglycemia in the smallest preterms), dosing.
7. **Diazoxide & Octreotide for Hyperinsulinism** *(mid-term)* — When to use, monitoring.
8. **Hydrocortisone for Adrenal Insufficiency** — *Cross-cluster with Cardio. Recommend home: Endocrine (the AI physiology), cross-link to Cardio's hypotension chapter.*

### Approach-to-problem chapters

9. **Approach to Neonatal Hypoglycemia** *(near-term, high-priority)* — PES vs AAP framework, transient vs persistent, when to push diazoxide. Strong opinion territory.
10. **Approach to Neonatal Hyperglycemia** *(near-term)* — The extreme-preterm case, insulin decision, when it's neonatal diabetes.
11. **Approach to Abnormal Newborn Screen Results** *(mid-term)* — Result categories, urgency by disorder, initial workup.
12. **Approach to Suspected Inborn Error of Metabolism** *(mid-term)* — Categories (urea cycle, organic acidemia, FAOD, MSUD), red flags, initial workup. You've engaged with this.
13. **Approach to Hypocalcemia** *(near-term)* — Early vs late, severity, treatment.
14. **Approach to Ambiguous Genitalia / DSD** *(mid-term)* — Initial workup, the multidisciplinary handoff, what NOT to do/say.

### Syndrome chapters

15. **Transient Hypoglycemia of the Newborn** *(near-term)* — IDM, IUGR, late preterm. Management.
16. **Persistent Hyperinsulinism** *(mid-term)* — Recognition, workup, treatment escalation to surgery.
17. **Infant of a Diabetic Mother (IDM)** *(near-term)* — Metabolic, cardiac, polycythemia, hypocalcemia, hypoglycemia.
18. **Congenital Adrenal Hyperplasia (CAH) & Salt-Wasting Crisis** *(mid-term)* — Recognition, acute management, follow-up.
19. **Congenital Hypothyroidism** *(mid-term)* — Newborn screen workflow, treatment initiation, transient vs permanent.
20. **Urea Cycle Defects (NICU Presentation)** *(mid-term)* — Hyperammonemia recognition and emergency management.
21. **Organic Acidemias (NICU Presentation)** *(mid-term)* — Acidosis with elevated anion gap, initial management.
22. **Fatty Acid Oxidation Defects** *(mid-term)* — Hypoketotic hypoglycemia, cardiomyopathy presentation.
23. **MSUD & Other Aminoacidopathies** *(long-term)* — Acute management of the decompensating infant.
24. **Galactosemia & Other Carbohydrate Disorders** *(long-term)* — Recognition, dietary intervention.
25. **Mitochondrial Disease (NICU Presentation)** *(long-term)* — Lactic acidosis, multi-system presentation.
26. **Neonatal Diabetes Mellitus** *(long-term)* — Transient vs permanent, KATP channel mutations.

### Cross-cluster decisions

- **Adrenal insufficiency / hydrocortisone:** Endocrine owns the physiology and primary chapter; Cardio cross-links from hypotension management.
- **Hypocalcemia:** Endocrine.
- **Hypomagnesemia:** Endocrine.
- **IEM with neuro presentation:** Endocrine owns the IEM chapters; Neuro's "approach to floppy infant" / "apparent HIE that isn't" cross-link.

### Suggested write order (Endo/Metabolic)

1. Approach to Neonatal Hypoglycemia
2. Neonatal Glucose Homeostasis (concept anchor)
3. Approach to Suspected Inborn Error of Metabolism
4. Approach to Abnormal Newborn Screen Results
5. Infant of a Diabetic Mother
6. Approach to Hypocalcemia
7. Congenital Adrenal Hyperplasia
8. Persistent Hyperinsulinism
9. Urea Cycle Defects (NICU Presentation)

---

## Cluster 9: Bilirubin & Hepatobiliary

### Scope

Neonatal jaundice (the dominant chunk), bilirubin neurotoxicity, cholestasis (cross-link to GI for biliary atresia detail), and exchange transfusion.

Reader: bedside clinician working through a TcB or TSB result, deciding on phototherapy timing, weighing exchange transfusion, or workup of direct hyperbili.

### Concept chapters

1. **Bilirubin Metabolism in the Newborn** *(mid-term)* — Production, conjugation, enterohepatic circulation. Why neonates jaundice.
2. **Bilirubin Neurotoxicity & Acute Bilirubin Encephalopathy** *(mid-term)* — Free bilirubin, BBB, the bind-and-deposit model. Foundation for thresholds.

### Modality chapters

3. **Phototherapy** *(near-term, high-priority)* — Mechanism, intensity, distance, eye protection, monitoring, when to stop.
4. **Exchange Transfusion: When & How** *(mid-term)* — Indications by BIND score / nomogram, technique, complications. Cross-link Heme.
5. **IVIG for Hemolytic Disease** *(mid-term)* — Indications, evidence (mixed), administration.

### Approach-to-problem chapters

6. **Approach to Indirect Hyperbilirubinemia** *(near-term, high-priority)* — The 2022 AAP nomogram, risk stratification, when to phototherapy.
7. **Approach to Direct (Conjugated) Hyperbilirubinemia** — *Lives in GI cluster; cross-link.*
8. **Approach to Prolonged Jaundice (>2 weeks)** *(mid-term)* — Differential, when to image, when to escalate.

### Syndrome chapters

9. **Physiologic vs Pathologic Jaundice** *(near-term)* — How to tell, when it's not physiologic.
10. **ABO Hemolytic Disease** *(near-term)* — Recognition, severity, management.
11. **Rh Hemolytic Disease** *(mid-term)* — Antenatal workup, postnatal management, ECN.
12. **G6PD Deficiency** *(mid-term)* — Recognition, triggers, management.
13. **Crigler-Najjar Syndrome** *(long-term)* — Type I vs II, recognition, lifelong management overview.
14. **Gilbert Syndrome** *(long-term)* — Recognition, reassurance.
15. **Breastmilk Jaundice vs Breastfeeding Jaundice** *(near-term)* — Distinguishing, management.
16. **Cephalohematoma-Associated Hyperbilirubinemia** *(mid-term)* — Recognition, monitoring intensity.
17. **Kernicterus / Chronic Bilirubin Encephalopathy** *(mid-term)* — Recognition, the post-acute syndrome.
18. **Biliary Atresia** — *Cross-cluster with GI. Recommend home: GI.*

### Cross-cluster decisions

- **Should Bilirubin be its own cluster or merged with GI?** Recommend its own cluster — bilirubin is the single most common NICU/nursery clinical issue and deserves its own home. The hepatobiliary content is small enough that it can ride along.
- **Hemolytic disease:** Heme owns hemolysis; Bilirubin owns the management.
- **Cholestasis:** GI owns the chapter; Bilirubin cross-links.

### Suggested write order (Bilirubin)

1. Approach to Indirect Hyperbilirubinemia (high-yield, universally relevant)
2. Phototherapy
3. Physiologic vs Pathologic Jaundice
4. ABO Hemolytic Disease
5. Exchange Transfusion: When & How
6. Approach to Prolonged Jaundice
7. Bilirubin Metabolism (concept anchor)
8. Breastmilk vs Breastfeeding Jaundice

---

## Cluster 10: Delivery Room & Resuscitation

### Scope

Fetal-neonatal transition, NRP and beyond, anticipation of high-risk deliveries, initial stabilization. Heavy cross-link with Cardio (transition physiology) and Pulmonary (lung aeration).

Reader: clinician walking to a high-risk delivery, or in the first 10 minutes after birth.

### Concept chapters

1. **Fetal-Neonatal Transition Physiology** *(near-term, high-priority)* — The respiratory, cardiac, and circulatory transitions. Cross-link to Cardio's hemodynamics chapter (overlap is OK; this one is transition-specific).
2. **Lung Aeration at Birth** *(mid-term)* — The Hooper model. First-breath physiology.
3. **Cord Management at Birth** *(near-term)* — Delayed cord clamping, cord milking, evidence and practice.

### Modality chapters

4. **The NRP Algorithm: Annotated** *(near-term, high-priority)* — Walk through the 2025 NRP algorithm with commentary, the evidence behind each step, the controversies.
5. **PPV in the Delivery Room** *(near-term)* — Mask seal, T-piece vs bag, PEEP, MR. SOPA. Why this is harder than it looks.
6. **Chest Compressions in the Newborn** *(mid-term)* — Technique, ratio, when to start, when to stop.
7. **Epinephrine in Neonatal Resuscitation** *(mid-term)* — Dose, route, timing, evidence.
8. **Volume Resuscitation in the Delivery Room** *(mid-term)* — When indicated, dose, fluid choice.

### Procedure chapters

9. **Intubation in the Delivery Room** — *Cross-link to Pulmonary cluster's intubation chapter.*
10. **Emergency UVC Placement** — *Cross-link to Cardio cluster's UVC chapter.*

### Approach-to-problem chapters

11. **Approach to the Non-Vigorous Newborn at Delivery** *(near-term)* — The first 60 seconds, what to do and in what order.
12. **Approach to the Meconium-Stained Newborn** *(near-term)* — The 2015+ algorithm shift, what still applies.
13. **Approach to the Anticipated Difficult Delivery** *(mid-term)* — Antenatally-known CDH, hydrops, severe IUGR, anticipated stridor. Pre-briefing the team.
14. **Approach to the Unexpected Anomaly at Delivery** *(mid-term)* — Stabilization-first principles, communication with family, transfer decisions.

### Syndrome chapters

15. **Failed Transition** *(mid-term)* — Persistent bradycardia, oxygenation failure, the differential.
16. **Severe Perinatal Asphyxia** *(near-term)* — Recognition, immediate cooling decision pathway (cross-link Neuro HIE).
17. **Stillbirth & Resuscitation Cessation** *(mid-term)* — When to stop, communication, post-event care of the family and team.

### Cross-cluster decisions

- **HIE recognition:** Resus owns the immediate-post-delivery framing; Neuro owns the syndrome.
- **Cooling decision:** Neuro owns; Resus cross-links from "Severe Perinatal Asphyxia."

### Suggested write order (Resus)

1. The NRP Algorithm: Annotated (foundation)
2. Approach to the Non-Vigorous Newborn
3. PPV in the Delivery Room
4. Fetal-Neonatal Transition Physiology
5. Cord Management at Birth
6. Approach to the Meconium-Stained Newborn
7. Severe Perinatal Asphyxia
8. Chest Compressions in the Newborn

---

## Cluster 11: Surgical Conditions (Cross-System Hub)

### Scope

NICU-facing management of surgical conditions. Pre-op, peri-op, post-op care. Surgical technique itself is out of scope (cross-link peds surgery resources).

Reader: bedside clinician managing a pre-op or post-op infant, working out what the surgeons did and what NICU care looks like.

### Concept chapters

1. **Pre-Operative Assessment in the Neonate** *(mid-term)* — Anesthesia risk, fluid status, hematologic optimization.
2. **Post-Operative Physiology in the Neonate** *(mid-term)* — Stress response, fluid shifts, ileus, pain management.

### Modality chapters

3. **Post-Operative Pain Management** *(near-term)* — Opioids, acetaminophen, regional. Dosing.
4. **NICU-Anesthesia Communication & Handoff** *(mid-term)* — What to ask, what to communicate, the OR-back-to-NICU bottleneck.

### Approach-to-problem chapters

5. **Approach to the Post-Operative Neonate** *(near-term)* — Systematic post-op review, expected vs concerning trajectory.
6. **Approach to Suspected Surgical Abdomen in the NICU** *(near-term)* — When to call surgery, what to image, what not to wait on.

### Syndrome chapters (post-op management focus)

7. **Congenital Diaphragmatic Hernia: Post-Op Management** — *Cross-link to Pulmonary's CDH chapter.*
8. **Gastroschisis: Post-Op Management** — *Cross-link to GI cluster.*
9. **Omphalocele: Post-Op Management** — *Cross-link to GI cluster.*
10. **Tracheoesophageal Fistula / Esophageal Atresia: Post-Op** — *Cross-link.*
11. **NEC: Surgical Course** — *Cross-link.*
12. **Posterior Urethral Valves: Post-Op** — *Cross-link.*
13. **Myelomeningocele: Post-Op** *(mid-term)* — Neurosurgical handoff, hydrocephalus surveillance.
14. **Congenital Lung Lesion Resection (CCAM/CPAM/Sequestration): Post-Op** *(long-term)* — Brief chapter.

### Cross-cluster decisions

- **Most surgical syndromes have their primary home in the relevant organ-system cluster** with this cluster owning only the surgical-management aspects. The pattern: GI cluster has "Gastroschisis: NICU Management" with the focus on feeding initiation; Surgical cluster has "Gastroschisis: Post-Op Management" with the focus on closure timing and complications. Heavy cross-linking. This may end up being just one chapter per condition; if so, primary home is the organ-system cluster.
- **Alternative model:** make Surgical a thin connective cluster with mostly cross-links, and let the syndrome chapters live entirely in their organ-system homes. Cleaner. Recommend this model.

### Suggested write order (Surgical)

Defer most of this cluster until fellowship rotations actually expose you to post-op management. Pre-fellowship priority: just the post-op pain management chapter.

---

## Cluster 12: Dermatology, Ophthalmology, Genetics & Miscellaneous

### Scope

Smaller content areas that don't warrant their own clusters. Skin, eyes, dysmorphology, and the topics that don't fit elsewhere.

### Dermatology

- **Newborn Skin Barrier & Premature Skin Care** *(mid-term)* — Concept-level.
- **Common Neonatal Rashes** *(mid-term)* — Erythema toxicum, transient neonatal pustular melanosis, milia, etc. Recognition, reassurance.
- **Vesicular Eruptions in the Newborn** *(near-term)* — HSV, varicella, bullous impetigo, EB, mastocytosis. The "when to call ID" chapter.
- **Vascular Lesions: Hemangiomas, Vascular Malformations** *(mid-term)* — Recognition, which need treatment, PHACE syndrome.
- **Subcutaneous Fat Necrosis** *(mid-term)* — Recognition, hypercalcemia surveillance.
- **Aplasia Cutis Congenita** *(long-term)* — Recognition, associated anomalies.

### Ophthalmology

- **Retinopathy of Prematurity (ROP): Screening & Recognition** *(mid-term)* — Screening criteria, what stages mean, when to escalate.
- **ROP: Treatment Options** *(mid-term)* — Laser, anti-VEGF, the bevacizumab debate.
- **Congenital Cataracts & Glaucoma** *(long-term)* — Recognition, urgency, workup.
- **Conjunctivitis: GC, Chlamydia, HSV, Chemical** — *Cross-link to ID.*

### Genetics & Dysmorphology

- **Approach to the Dysmorphic Newborn** *(mid-term)* — A pattern recognition primer, what to consult, what to test.
- **Trisomy 21: NICU-Relevant Issues** *(near-term)* — AVSD, duodenal atresia, hypothyroidism, polycythemia, leukemoid reaction.
- **Trisomy 18 & 13** *(mid-term)* — Recognition, prognosis conversation, scope-of-care discussions.
- **Turner Syndrome** *(long-term)* — Recognition, cardiac and renal screening.
- **22q11 Deletion (DiGeorge)** *(mid-term)* — Cardiac, hypocalcemia, thymus.
- **Beckwith-Wiedemann** *(mid-term)* — Hypoglycemia, surveillance.
- **VACTERL Association** *(mid-term)* — Workup pathway.

### Audiology / Hearing

- **Universal Newborn Hearing Screen & Follow-Up** *(mid-term)* — Pass/fail framework, urgency of follow-up.

### Suggested write order (Misc)

Defer most of this cluster. Pre-fellowship priority: Vesicular Eruptions (HSV recognition) and Trisomy 21 NICU issues if cases bring them up.

---

## Cross-cutting content (not its own cluster)

### Guide to NICU Bedside Care (the Farkas "supportive care" analog)

Single long meta-chapter, cross-linked everywhere. Sections:

- **Thermoregulation** — incubator settings, kangaroo care, hypo/hyperthermia thresholds
- **Line care basics** — site care, dressing changes, securement
- **Routine monitoring** — what alarms mean, when to act
- **Sedation & analgesia framework** — opioid selection, withdrawal, when to use, when not
- **Developmental care** — clustered care, light, noise, positioning
- **Family-centered care** — communication, presence at rounds, breaking bad news
- **Feeding support basics** — kangaroo care for feeding, NNS, transitioning to PO
- **Skin care universals** — adhesives, prepping for tape, lines

This chapter is non-trivial to write but high-yield because it offloads universal content from every syndrome chapter.

### Drug Handbook

A separate section of the site (like Farkas's). Each drug gets a short structured page: indications, dosing by GA/weight, route, monitoring, contraindications, neonatal-specific considerations. Long-term project — not a near-term priority. May initially just point to Neofax + commentary on where you'd diverge.

### Procedures Hub

Cross-link page listing all procedure chapters. Useful for the "I need to know how to do X right now" use case. No original content — pure navigation.

---

## Project-level priority across all clusters

If you had to rank what gets written first across the whole project, integrating the per-cluster recommendations:

**Tier 1 (the universally-relevant flagships — write in fellowship Y1):**

1. hsPDA (cardio — already drafted)
2. Neonatal Hemodynamics Fundamentals (cardio)
3. Approach to Suspected Early-Onset Sepsis (ID)
4. NEC: Recognition & Medical Management (GI)
5. RDS (pulm)
6. Approach to Indirect Hyperbilirubinemia (bili)
7. HIE: Recognition & Initial Management (neuro)
8. Approach to Neonatal Hypoglycemia (endo)
9. Approach to Thrombocytopenia (heme)
10. The NRP Algorithm: Annotated (resus)

These 10 chapters, if they existed, would already give the site a real identity. Realistic in fellowship year 1 if you batch by cluster during relevant rotations.

**Tier 2 (deepens existing strengths and builds infrastructure — Y2):**

11–25. The remaining "near-term" chapters from each cluster's suggested write order. ~15 chapters across the year.

**Tier 3 (fills out the resource — Y3 and beyond):**

The "mid-term" chapters across all clusters. ~30–50 chapters spread across late fellowship and early attending years.

**Tier 4 (long-term / cases-force-it):**

Everything marked long-term. Written as cases come up, not on a schedule.

Total mature site: roughly **120–150 chapters**. Comparable to current IBCC scope. Achievable over a 5–7 year arc if cluster batching aligns with rotations and clinical work.

---

## What this document is for

- A single reference for project scope. When you encounter a topic and wonder "does this belong on the site, and if so where?" — check here.
- A scaffold for the cluster `_index.md` landing pages. Each cluster's landing page is essentially a polished, public version of that cluster's section in this document.
- A planning anchor for what to write next. The "suggested write order" sections collapse decision fatigue.
- An honest reality check on scope. 120-150 chapters is a 5-7 year project. Pacing matters.

What this document is **not**:

- A commitment. Reorganize freely as fellowship cases and your interests evolve. The clustering will not survive contact with reality, and that's fine.
- Exhaustive. Topics I've missed will surface. Add them.
- A writing schedule. The "near-term / mid-term / long-term" tags are rough.

This is the scope of the project I've been working on. Cross-link with `cardiac-section-architecture.md` for the cardiac deep-dive.
