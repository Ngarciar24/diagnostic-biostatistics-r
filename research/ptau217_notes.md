# Elecsys Phospho-Tau (217P) Plasma (pTau217): verified public facts

Compiled 2026-10-16. Only facts read directly from the sources below are listed as verified. Items marked "derived" are my arithmetic on verified counts.

Source keys:
- **FDA-DS** = FDA 510(k) Decision Summary K261686, 37 pp. https://www.accessdata.fda.gov/cdrh_docs/reviews/K261686.pdf (PDF opened and text extracted; page numbers are the "K261686 - Page n of 37" footers; the footer sits at the bottom of each page, so text above a footer is on that page).
- **FDA-DB** = 510(k) database record for K261686, read through the openFDA mirror https://api.fda.gov/device/510k.json?search=k_number:K261686 (the accessdata pmn.cfm page itself blocked automated access, so it was not opened directly).
- **ROCHE-0824** = Roche investor update/media release, 24 Aug 2026. https://www.roche.com/investors/updates/inv-update-2026-08-24
- **ROCHE-CE** = https://www.roche.com/media/releases/med-cor-2026-05-12
- **ROCHE-BDD** = https://www.roche.com/media/releases/med-cor-2024-04-11
- **HIBAR** = Hibar et al., PMC12805464, https://pmc.ncbi.nlm.nih.gov/articles/PMC12805464/
- **HORTSCH** = Hortsch et al., PMC13053736, https://europepmc.org/article/MED/41887009 (full text via Europe PMC REST for PMC13053736)

## 0. Citation checks (user-supplied citations)

| Citation | Result |
|---|---|
| Hibar et al. 2026, Alzheimer's & Dementia 22(1):e71009 | Correct. Hibar DP, Bauer A, Rabe C, Borlinghaus N, Jethwa A, Kollmorgen G, Di Domenico A, Zetterberg H, Blennow K, Masters CL, Sperling RA, Bittner T. "Elecsys pTau217 plasma immunoassay detection of amyloid pathology in clinical cohorts." Alzheimers Dement 2026 Jan 15;22(1):e71009. DOI 10.1002/alz.71009. PMID 41537338, PMCID PMC12805464. |
| Hortsch et al. 2026, J Prev Alzheimers Dis 13(5):100534 | Correct. Hortsch S, Di Domenico A, Borlinghaus N, Caley D, Kaminioti-Dumont L, Jeppesen SB, Gonzalez-Escalante A, Ritchie C, Frederiksen KS, Suarez-Calvet M. "Performance of a fully automated plasma tau phosphorylated at threonine 217 immunoassay to reflect amyloid-beta burden in an unselected cohort representative of clinical practice." J Prev Alzheimers Dis 2026;13(5):100534 (issue dated May 2026; epub 25 Mar 2026). DOI 10.1016/j.tjpad.2026.100534. PMID 41887009. Source: Europe PMC record. |
| Roche media release dated 24 Aug 2026 | Date confirmed (ROCHE-0824, "Basel, 24 August 2026"). Note the FDA decision date is earlier: 2026-08-19 (FDA-DB). |

Important caveats on the two papers (both Roche-authored/affiliated, both use the PROTOTYPE assay, "not approved for clinical use" per HIBAR):
- Neither paper reports the FDA-cleared cut-offs (0.223 / 0.378 pg/mL).
- HIBAR uses a single rule-out cut-off (0.189 pg/mL) and no intermediate zone. HORTSCH uses an exploratory 90% PPA / 90% NPA double cut-off. Neither is the pivotal data behind the FDA clearance.
- The pivotal clearance data are in FDA-DS only.

## 1. Regulatory facts

| Item | Value | Source |
|---|---|---|
| 510(k) number | K261686 | FDA-DS p.1; FDA-DB |
| Device / applicant | Elecsys Phospho-Tau (217P) Plasma; Roche Diagnostics (Indianapolis, IN) | FDA-DS p.1; FDA-DB |
| Date received / decision | 2026-05-21 / 2026-08-19; decision code SESE (Substantially Equivalent); Traditional 510(k) | FDA-DB |
| Product code / regulation / class | SET; 21 CFR 866.5840 "Alzheimer's Disease Pathology Assessment Test"; Class II; panel IM | FDA-DS p.1 |
| Predicate | Lumipulse G pTau 217/beta-Amyloid 1-42 Plasma Ratio, K242706 | FDA-DS p.4 |
| Instrument | cobas pro e 801 (K191899); ECLIA, 18-min test time, 60 uL sample; K2/K3-EDTA plasma | FDA-DS pp.2-3 |
| Indication for use | Aid in identifying patients with amyloid pathology presenting with signs, symptoms, or complaints of cognitive decline associated with Alzheimer's disease; plasma from individuals aged 55 years and older; result must be used in the diagnostic pathway with other clinical information; Rx only | FDA-DS p.2 |
| Monitoring / dementia prediction exclusion | NOT in the FDA decision summary text. Stated in Roche release: "not intended to be used as a stand-alone test"; safety and effectiveness not established for predicting dementia or other neurologic conditions, nor for monitoring effect of therapeutic products. Full labeling (IFU) not opened. | ROCHE-0824 |
| Roche "rule-in and rule-out with the same cutoffs in primary and specialty care" | Roche claim ("first and only FDA-cleared single-biomarker blood test"); Roche release gives no numeric cut-offs or performance | ROCHE-0824 |
| Breakthrough Device Designation | Roche release 11 Apr 2024; then-intended use age 60 and older; "in development and not yet approved" | ROCHE-BDD |
| CE mark | Roche release 12 May 2026; retrospective data; same high/low cutoffs in primary and secondary care; no numbers given | ROCHE-CE |
| FDA press announcement | None found; only the 510(k) database/decision summary and Roche/trade coverage | searches |

## 2. Cut-offs and result categories (FDA-DS p.3, interpretation table; units pg/mL)

| Category | Rule | Interpretation (labeling) |
|---|---|---|
| Positive | pTau217 > 0.378 pg/mL | high likelihood of amyloid pathology |
| Intermediate | > 0.223 and <= 0.378 pg/mL | indeterminate; consider further testing |
| Negative | pTau217 <= 0.223 pg/mL | low likelihood; investigate other causes |

- Footnote on p.3: lower PPV expected in low-prevalence (primary care) settings; positives near the upper cut-off may need further evaluation or specialist follow-up.
- Cut-off derivation (FDA-DS p.20, "Assay Cut-Off"): 687 banked K2-EDTA samples (primary care N=194, 28.2%; secondary/tertiary N=493, 71.8%); mean age 71.7 (61.0-86.0); 286 (41.6%) PET positive, 401 (58.4%) PET negative; prevalence 21.1% (41/194) primary and 49.7% (245/493) secondary/tertiary. The text states the cut-offs were "selected" but does not state the selection rule (target sensitivity/specificity not verified).
- Analytic: LoB 0.047, LoD 0.056, LoQ 0.056 pg/mL (claimed) (FDA-DS p.20 area). Calibrators approx 0.14 and 2.00 pg/mL (p.3).
- The two cut-offs fall within the measuring range near the LoQ-to-low-range; the lower cut-off 0.223 is about 4x the LoQ.

## 3. Pivotal clinical performance (FDA-DS pp.22-27)

Design: prospective-retrospective banked samples from two cohorts (APPROACH, 16 sites US/Europe, primary and secondary/tertiary care; AACI phase III trial screening samples, US secondary/tertiary). N = 958 with valid assay and PET results; mean age 71.1 (55-85); cognitive complaints or impairment of unknown cause; 876 (91.4%) US sites; 234 (24.8%) primary care (pp.22-23; note p.24-25 table gives primary n=238, 24.8%); MMSE 28-30 N=295, 25-27 N=363, 22-24 N=227, <22 N=73.
Reference standard (p.25): amyloid PET visual read with FDA-approved tracers (18F-florbetapir, 18F-florbetaben, 18F-flutemetamol), six trained blinded readers (three from each of two vendors); positive if >=4 of 6 positive; negative if <=2; 3-3 split broken by excluding the reader with lowest CSF agreement and majority of remaining five; any non-readable read makes the scan missing. Result: 378 (39.5%) positive, 580 (60.5%) negative. 3-3 splits 84 (8.77%). Mean inter-reader PPA 83.6%, NPA 91.3%, OPA 87.3%. Blood-to-PET interval mean 37.7 d (SD 28.9), median 30 d. CSF was not the truth standard (used only for tie-break). No centiloid threshold used in the pivotal analysis.

### 3.1 Three-category contingency (FDA-DS p.26, table)

| Assay result | PET positive | PET negative | Total |
|---|---|---|---|
| Positive (> 0.378) | 285 | 37 | 322 |
| Intermediate (0.223 < x <= 0.378) | 72 | 119 | 191 |
| Negative (<= 0.223) | 21 | 424 | 445 |
| Total | 378 | 580 | 958 |

### 3.2 Reported performance (FDA-DS pp.26-27)

| Metric | Estimate | 95% CI | Source location |
|---|---|---|---|
| PPA (positive result among PET+; intermediates counted as not-positive) | 75.4% (285/378) | 70.8%, 79.5% | p.27 text |
| NPA (negative result among PET-; intermediates counted as not-negative) | 73.1% (424/580) | 69.4%, 76.6% | p.27 text |
| PPV of positive result ("PV") | 88.5% (285/322) | 84.9%, 91.4% | p.27 table and text |
| PV of intermediate | 37.7% (72/191) | 31.7%, 44.0% (table prints "317%"; text prints 31.7%) | p.27 |
| PV of negative (post-test probability of PET+) | 4.7% (21/445) | 3.2%, 6.9% | p.27 |
| NPV of negative result | 95.3% (424/445) | 93.1%, 96.8% | p.27 text |
| Frequency positive / intermediate / negative | 33.6% (322/958) / 19.9% (191/958) / 46.5% (445/958) | not given | p.27 (table denominators print 959; counts total 958) |
| LR+ (positive category) | 11.82 | 8.65, 16.25 | p.27 |
| LR (intermediate) | 0.93 | 0.71, 1.20 | p.27 |
| LR- (negative category) | 0.08 | 0.05, 0.11 | p.27 |
| Prevalence of PET positivity | 39.5% (378/958) | n/a | p.27 |

Derived by me from the p.26 counts (NOT stated in FDA-DS; no CI computed): sensitivity of the rule-out step (not-negative among PET+) = 357/378 = 94.4%; specificity of the rule-in step (not-positive among PET-) = 543/580 = 93.6%; intermediate zone = 191/958 = 19.9% (matches).

### 3.3 Subgroups (FDA-DS pp.28-35; predictive value of each category with 95% CI, n/N)

| Subgroup | Positive PV | Intermediate PV | Negative PV (PET+ among negatives) | Intermediate frequency | Page |
|---|---|---|---|---|---|
| Age 55-70 (N=430, prev 25.1%) | 86.4% (76/88; 78.4-91.8) | 29.8% (25/84; 21.8-38.8) | 2.7% (7/258; 1.3-5.2) | 19.5% (84/430) | p.30 |
| Age 71-85 (N=528, prev 51.1%) | 89.3% (209/234; 85.3-92.4) | 43.9% (47/107; 35.8-52.4) | 7.5% (14/187; 4.6-11.8) | 20.3% (107/528) | pp.30-31 |
| Primary care (N=238, prev 21.4%) | 78.3% (36/46; 66.1-87.0) | 27.7% (13/47; 17.7-39.4) | 1.4% (2/145; 0.4-4.5) | 19.7% (47/238) | p.32 |
| Secondary/tertiary (N=720, prev 45.4%) | 90.2% (249/276; 86.5-93.0) | 41.0% (59/144; 34.0-48.3) | 6.3% (19/300; 4.2-9.4) | 20.0% (144/720) | p.32 |
| MMSE 28-30 (N=295, prev 26.4%) | 77.3% (51/66; 67.3-85.0) | 26.9% (21/78; 19.2-35.7) | 4.0% (6/151; 1.9-7.9) | 26.4% | p.28 |
| MMSE 25-27 (N=363, prev 38.8%) | 90.4% (103/114; 84.2-94.4) | 40.8% (31/76; 31.4-50.7) | 4.0% (7/173; 2.0-7.8) | 20.9% | pp.28-29 |
| Male (N=431, prev 40.4%) | 84.7% (122/144; 78.8-89.3) | 38.5% (40/104; 30.6-46.7) | 6.6% (12/183; 3.9-10.7) | 24.1% | pp.29-30 |
| Female (N=527, prev 38.7%) | 91.6% (163/178; 87.0-94.7) | 36.8% (32/87; 28.1-46.3) | 3.4% (9/262; 1.8-6.2) | 16.5% | p.30 |
| White (N=811, prev 44.8%) | 89.9% (276/307; 86.4-92.6) | 41.6% (69/166; 35.0-48.3) | 5.3% (18/338; 3.4-8.1) | 20.5% | p.31 |
| Black/African American (N=110) | 54.5% (6/11; 30.2-75.7) | 10.5% (2/19; printed CI 3.1-5.9 is inconsistent with the point estimate) | 3.8% (3/80; 1.4-7.6) | 17.3% | p.31-32 |

- Kidney function: the FDA-DS has NO eGFR-stratified analysis. The only renal item is a "kidney disease" comorbidity subgroup (2.7% affected, N=24): Positive PV 100% (3/3; 46.5-100), Intermediate PV 0% (0/7; 0-24.6), Negative PV 7.1% (1/14; 1.4-19.5), intermediate frequency 29.2% (7/24) (pp.33-34). Too small to support any claim. Statement that performance is "similar regardless of comorbidity" (p.35) is the sponsor's.
- Other comorbidities (cardiovascular N=500, hypertension 475, etc.), tabulated on pp.34-35; intermediate frequency ranges 14.5%-29.2% across comorbidity strata.
- Age-related reference interval (p.36): cognitively normal N=167 (aged 55-80), QDRS 0; 95% reference interval 0.0832-0.628 pg/mL; 68.3% <= 0.223; 22.8% in 0.223-0.378; 8.98% > 0.378. By age: 55-70 y 4.88% above 0.378; 71-80 y 20.5% above 0.378 (p.36).
- FDA-DS gives no stratified results by eGFR or by amyloid PET threshold (no centiloid analysis).

### 3.4 Statistical methods stated in FDA-DS
- CI method for PPA/NPA: NOT stated.
- PV 95% CIs: "calculated based on 95% CIs of corresponding likelihood ratios" (p.26 footnote); LR CIs "calculated using an asymptotic method for ratios of two independent binomial proportions" (p.26). This is not Clopper-Pearson or Wilson.
- Indeterminates: reported as their own category (the intermediate row), not excluded; PPA/NPA treat intermediates as misclassified (denominator all 378/580). Only PET-unreadable scans are excluded (missing). A count of PET-missing/excluded subjects was not verified.
- No pre-specified performance goals, sample-size calculation, or hypothesis test other than the CI-vs-prevalence comparison for PV (p.27) were found in the text read.

### 3.5 Internal inconsistencies in FDA-DS (for transparency; do not copy uncritically into teaching material)
1. p.26 says "pre-specified cut-offs of 0.225 pg/mL and 0.378" but the table and labeling use 0.223.
2. p.26 says "prevalence ... was 13.1%" in one sentence, but 39.5% everywhere else.
3. Frequencies use denominator 959 while counts total 958; p.22-23 table lists primary n=238 vs "234" in the narrative.
4. Table prints intermediate PV CI as "317%, 44.0%".
5. Black/African American intermediate PV 10.5% (2/19) has printed CI 3.1-5.9%, impossible; the point estimate 2/19 is 10.5%.
6. p.35 reference-interval paragraph names "Elecsys Phospho-Tau (181P)" once, and "71 to 85 years" vs table "71 to 80 years".
7. NPA/PPA CIs vs "PV" CIs use different methods.

## 4. Hibar et al. 2026 (prototype assay; Table/page refs are PMC12805464 sections)

| Item | Value | Source location |
|---|---|---|
| Design | Retrospective analysis; five cohorts (A4, SKYLINE, AIBL, CREAD, CREAD2); prototype Elecsys Phospho-Tau 217P on cobas e 801, "not approved for clinical use" | Methods |
| N | 2,148 total: 538 cognitively impaired (CI; AIBL 124, CREAD 197, CREAD2 217) and 1,610 cognitively unimpaired (CU; A4 830, SKYLINE 319, AIBL 461); 7,252 eligible | Methods, Table 1 |
| Reference standard | Amyloid PET visual read per package insert (Amyvid, Vizamyl, Neuraceq); secondary Centiloid >= 24 and >= 40. CSF not used as truth. Age 50-90, plasma within 12 months of PET | Methods |
| Single rule-out cut-off | < 0.189 pg/mL (units pg/mL); no intermediate zone; no rule-in cut-off | Table 2 |
| CI group at < 0.189 (n=538; TP 390, FN 4, FP 102, TN 42) | Sens 98.98%, Spec 29.17%, NPV 92.51% (prevalence-adjusted to 69.9%), PPV 76.48%, screen-out 9.48% | Table 2 |
| CU group (n=1,610; TP 214, FN 10, FP 683, TN 703) | Sens 95.54%, Spec 50.72%, NPV 98.60%, PPV 23.86%, screen-out 44.29% | Table 2 |
| AUC visual read (95% CI) | CI 0.878 (0.840-0.915); CU 0.907 (0.885-0.929) | Results |
| AUC CL>=24 / CL>=40 | CI 0.872 (0.828-0.917) / 0.849 (0.807-0.891); CU 0.864 (0.842-0.887) / 0.911 (0.892-0.930) | Results |
| Not reported | CIs for sens/spec/NPV/PPV; CI method; eGFR; age-stratified performance; intermediate fraction | not verified in text read; supplementary Tables S1-S10 not opened |
| Software | R 4.3.1, stats4phc 0.1.2 | Methods |

(Note: the extraction tool reported that the final ~3,400 characters of the PMC page, i.e. references/end matter, were not read.)

## 5. Hortsch et al. 2026 (prototype assay, APPROACH cohort)

| Item | Value | Source location |
|---|---|---|
| Design | Prospective, multicenter, consecutive enrolment, 12 sites (primary and secondary care, Europe and US), May 2023 - Mar 2024; ages 55-80 with cognitive complaints; K2-EDTA plasma | Methods 2.1 |
| N | 604 recruited; 588 analysed; SCD 189, MCI 352, mild dementia 40, no diagnosis 7 | Methods 2.1 / Table 1 |
| Reference standard | Amyloid PET, quantitative centiloid classification at cut-offs 24.1, 30, 40, 50 (not visual read); tracers: florbetaben 298 (50.7%), florbetapir 263 (44.7%), flutemetamol 27 (4.59%). Blood-to-PET interval mean 56.1 d, median 49 d (range -48 to 192). CSF (pTau181/Abeta42) available in a subset; not the truth standard | Methods, Table 1 |
| Prevalence of PET positivity | 33.2% (CL 24.1), 30.4% (CL 30), 26.7% (CL 40), 25.3% (CL 50) | 3.3 |
| AUC | peak 0.933 at CL 32; 0.925 overall at CL 30; SCD 0.914, MCI 0.918, mild dementia 0.920 | 3.3, 3.4 |
| Double cut-off | lower cut-off set at 90% PPA, upper cut-off at 90% NPA; results positive/negative/indeterminate; indeterminate 5.78% at CL 30; <15% at all CL cut-offs | Methods; 3.3 (Table S7) |
| PPA/NPA CI method | two-sided 95% CIs, Wilson score method, for cut-offs 0.250-0.800 pg/mL in steps of 0.025 | Methods |
| Kidney function | eGFR (CKD-EPI 2021, creatinine Jaffe) groups: G1+G2 (>=60) 514 (87.4%), G3a 58 (9.86%), G3b 8 (1.36%), G4+G5 5 (0.85%), missing 3. Higher pTau217 with worse kidney function; G4-G5 had >1.0 pg/mL and false positives vs CL 30 in 4/588 (<1%) | Table 1; 3.4 / Fig 3C |
| Age and sex | subgroup analysis by age (55-64, 65-74, 75-80) and sex is graphical (Figs S4-S5); numeric tables not opened | 3.4 |
| Not verified | the numeric double cut-off values, PPA/NPA with CIs at them (supplementary tables S3-S9 not opened) | |

## 6. Methods citations (verified via Europe PMC/Crossref records; abstracts read)

| Citation | Verified record | What it says (abstract) |
|---|---|---|
| Coste J, Pouchot J. 2003 | "A grey zone for quantitative diagnostic and screening tests." Int J Epidemiol 32(2):304-313. DOI 10.1093/ije/dyg054, PMID 12714554 | Proposes a three-zone partition with a grey zone between positive and negative; width depends on separation of means, variability (biological and measurement) and the accepted misclassification risks; illustrated with tuberculin test and iron-deficiency markers. |
| Buderer NMF. 1996 | "Statistical methodology: I. Incorporating the prevalence of disease into the sample size calculation for sensitivity and specificity." Acad Emerg Med 3(9):895-900. DOI 10.1111/j.1553-2712.1996.tb03538.x, PMID 8870764 | Sample size for sensitivity and specificity from desired precision, hypothesised Se/Sp and disease prevalence; gives tables. (Initials "NMF" not verified in the record; Europe PMC lists "Buderer NM".) |
| Flahault A, Cadilhac M, Thomas G. 2005 | "Sample size calculation should be performed for design accuracy in diagnostic test studies." J Clin Epidemiol 58(8):859-862. DOI 10.1016/j.jclinepi.2004.12.009, PMID 16018921 | Tables of number of cases for expected sensitivity 0.60-0.99, acceptable lower 95% limit 0.50-0.98, with 5% probability the estimated lower limit falls below the acceptable level. |
| Hanley JA, McNeil BJ. 1982 | "The meaning and use of the area under a receiver operating characteristic (ROC) curve." Radiology 143(1):29-36. DOI 10.1148/radiology.143.1.7063747, PMID 7063747 | AUC equals probability a random diseased case is ranked above a random non-diseased case (Wilcoxon); gives standard error formulas and sample size guidance. |
| Obuchowski NA. 2000 | "Sample size tables for receiver operating characteristic studies." AJR Am J Roentgenol 175(3):603-608. DOI 10.2214/ajr.175.3.1750603, PMID 10954438 | Tables for multi-observer ROC studies comparing two imaging techniques; this is the 2000 paper matched to "Obuchowski 2000s". Earlier: Obuchowski, "Computing sample size for ROC studies," Invest Radiol 1994;29(2):238-243. The user's reference is ambiguous (which year/paper); not resolved. |
| DeLong ER, DeLong DM, Clarke-Pearson DL. 1988 | "Comparing the areas under two or more correlated receiver operating characteristic curves: a nonparametric approach." Biometrics 44(3):837-845. DOI 10.2307/2531595, PMID 3203132 | Nonparametric comparison of correlated AUCs using generalized U-statistics covariance estimate. |
| Clopper CJ, Pearson ES. 1934 | "The use of confidence or fiducial limits illustrated in the case of the binomial." Biometrika 26(4):404-413. DOI 10.1093/biomet/26.4.404 (Crossref) | Exact binomial confidence limits. Abstract not read (Crossref metadata only). |
| Wilson EB. 1927 | "Probable inference, the law of succession, and statistical inference." J Am Stat Assoc 22(158):209-212. DOI 10.1080/01621459.1927.10502953 (Crossref) | Score interval for a binomial proportion. Abstract not read (Crossref metadata only). |
| Zhou XH, Obuchowski NA, McClish DK. | "Statistical Methods in Diagnostic Medicine", Wiley. 1st ed. 2002 (ISBN 9780471347729); 2nd ed. 2011 (ISBN 9780470183144; DOI 10.1002/9780470906514) per Crossref. Edition to cite is the course's choice; 2nd ed. 2011 is current. | Textbook; content not opened. |
| Pepe MS. 2003 | "The Statistical Evaluation of Medical Tests for Classification and Prediction." Oxford University Press, 2003 (ISBN 9780198509844 hardback; 9780198565826 paperback per Open Library). DOI 10.1093/oso/9780198509844.001.0001 (Crossref) | Textbook; content not opened. |

## 7. Not verified

- FDA 510(k) database page itself (pmn.cfm) and any FDA press announcement: not opened/not found (site blocked automated requests; openFDA mirror used).
- Final FDA labeling (instructions for use): not seen; therefore the monitoring/dementia-prediction exclusion is verified only from the Roche release, not the decision summary. The decision summary indication is silent on monitoring.
- How the cut-offs 0.223 and 0.378 were chosen (no target Se/Sp stated; p.20).
- CI method for PPA/NPA in FDA-DS; any sample size justification or pre-specified acceptance criteria.
- eGFR-stratified performance in the FDA pivotal data (absent); Hortsch has eGFR distribution but no verified numeric performance by eGFR group beyond the 4/588 false-positive statement.
- Hibar supplementary Tables S1-S10 and Hortsch Tables S1-S9 (numeric cut-offs, Wilson CIs, age/sex tables).
- Intermediate-zone fraction for Hibar (single cut-off design).
- Sensitivity/specificity (versus PPA/NPA) with CIs for the cleared two-cut-off scheme: not reported in FDA-DS; only my derived 94.4% and 93.6% (no CI).
- Number of PET-missing or excluded subjects in the pivotal study.
- Clopper-Pearson, Wilson, Zhou et al., Pepe: abstracts/contents not read.
- Whether Roche's 24 Aug 2026 release PDF attachment contains any numbers: the page text shows none; the PDF attachment was not read.
