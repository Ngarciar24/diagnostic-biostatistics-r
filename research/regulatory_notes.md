# Regulatory notes (verified against primary sources)

Verification date for everything below: **2026-10-16**. Method: documents opened and read in full text (EUR-Lex HTML, FDA PDFs/web pages, ISO committee page, PubMed E-utilities record, ICH PDFs, CDISC pages). Anything not opened is labelled **not verified**. Quotes are verbatim and short.

Chapter mapping assumed for the ledger (change if your TOC differs): ch1 = regulatory landscape / definitions; ch5 = diagnostic accuracy design, reporting, agreement metrics; ch8 = companion diagnostics and codevelopment; ch9 = study protocol / SAP / estimands / data standards.

Source-text caveat: the EUR-Lex text I read is the original OJ text of Reg. (EU) 2017/746 (CELEX 32017R0746, https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=CELEX:32017R0746, reachable after retries). The consolidated version (CELEX 02017R0746-20250110) returned HTTP 202 with an empty body, so **not verified** against the consolidated text. Transitional amendments were verified from the amending acts' own text (2022/112, 2024/1860). Article/Annex numbering of the provisions cited below is unaffected by those amendments, but a later amendment could have altered wording: check the consolidated text before quoting in teaching material.

---

## 1. EU IVDR - Regulation (EU) 2017/746

URL (ELI): https://eur-lex.europa.eu/eli/reg/2017/746/oj

### 1.1 Article 2 definitions (point numbers)

| Point | Term | Verbatim (<=25 words) |
|---|---|---|
| 2(7) | companion diagnostic | "a device which is essential for the safe and effective use of a corresponding medicinal product to:" (a) identify patients "most likely to benefit"; (b) identify patients "likely to be at increased risk of serious adverse reactions" |
| 2(36) | clinical evidence | "clinical data and performance evaluation results, pertaining to a device of a sufficient amount and quality" to allow qualified assessment of safety and intended clinical benefit |
| 2(38) | scientific validity of an analyte | "the association of an analyte with a clinical condition or a physiological state" |
| 2(39) | performance of a device | "It consists of the analytical and, where applicable, the clinical performance supporting that intended purpose" |
| 2(40) | analytical performance | "the ability of a device to correctly detect or measure a particular analyte" |
| 2(41) | clinical performance | "the ability of a device to yield results that are correlated with a particular clinical condition or a physiological or pathological process or state" (+ "in accordance with the target population and intended user") |
| 2(42) | performance study | "a study undertaken to establish or confirm the analytical or clinical performance of a device" |
| 2(44) | performance evaluation | "an assessment and analysis of data to establish or verify the scientific validity, the analytical and, where applicable, the clinical performance of a device" |
| 2(46) | interventional clinical performance study | test results "may influence patient management decisions and/or may be used to guide treatment" |
| 2(49) / 2(50) / 2(51) | diagnostic specificity / diagnostic sensitivity / predictive value | defined in the Regulation (useful for ch5: IVDR uses "diagnostic sensitivity/specificity", Annex I 9.1(b) adds likelihood ratio) |

Note: there is no separate definition of "scientific validity" of a device; the definition is of "scientific validity **of an analyte**" (point 38).

### 1.2 Articles 47-48 - what they actually cover
- **Art. 47 = Classification of devices** (not safety/performance requirements). Art. 47(1): "Devices shall be divided into classes A, B, C and D". Classification per Annex VIII; disputes, reclassification by implementing act.
- **Art. 48 = Conformity assessment procedures** (class-specific routes via Annexes IX-XI; class D, C, B, A in paras 3-10; para 11: performance-study devices fall under Arts 57-77).
- The GSPR themselves are in **Annex I** (and Art. 5 requires compliance with them). Performance-characteristic requirements are Annex I Chapter II, Section 9.

### 1.3 Articles 56-58
- **Art. 56 - "Performance evaluation and clinical evidence".** Conformity with Annex I GSPR "shall be based on scientific validity, analytical and clinical performance data" (56(1)); manufacturer must plan, conduct and document performance evaluation per Art. 56 and Annex XIII Part A; 56(3) three pillars: scientific validity, analytical performance, clinical performance; 56(4) "Clinical performance studies ... shall be carried out unless it is duly justified to rely on other sources"; 56(5) documented in the performance evaluation report (Annex XIII Part A 1.3.2); 56(6) updated with PMPF data (Part B) and **PE report for class C and D "at least annually"**.
- **Art. 57 - "General requirements regarding performance studies".** Study design/conduct: rights, safety, dignity, well-being of subjects "prevail over all other interests", data "scientifically valid, reliable and robust" (57(3)); data-protection law applies to left-over-sample studies.
- **Art. 58 - "Additional requirements for certain performance studies".** Applies to (a) surgically invasive sampling only for study, (b) interventional clinical performance studies (Art. 2(46)), (c) studies with additional invasive procedures or risks -> must also follow Arts 59-77 and Annex XIV. **58(2): studies involving companion diagnostics are subject to the same requirements**, except CDx studies using only left-over samples, which "shall however be notified to the competent authority". 58(3): scientific and ethical review, at least one lay person.
- (Arts 59-77 = authorisation, conduct, registration etc. of performance studies, not read in detail.)

### 1.4 Annex I (GSPR)
Structure: Chapter I General requirements (Sections 1-8; risk management Section 3); Chapter II Requirements regarding performance, design and manufacture (Sections 9-19); Chapter III Information supplied with the device (Section 20 and following).
- **Section 9.1(a)** analytical performance list: "analytical sensitivity, analytical specificity, trueness (bias), precision ..., limits of detection and quantitation, measuring range, linearity, cut-off".
- **Section 9.1(b)** clinical performance: "diagnostic sensitivity, diagnostic specificity, positive predictive value, negative predictive value, likelihood ratio, expected values in normal and affected populations".
- 9.3 metrological traceability; 9.4 self-testing / near-patient (layperson) performance.
These are the statistical parameters that map to the Chapter 5 metrics.

### 1.5 Annex VIII - classification (Chapter 2 rules)
- Rule 1 -> class **D** (transmissible agents in blood/tissue donations; life-threatening high-propagation agents; viral load in life-threatening disease).
- Rule 2 -> class **C** (blood grouping / tissue typing), but **D** for ABO, Rhesus, Kell, Kidd, Duffy markers.
- **Rule 3 -> class C**, items (a)-(m). **Companion diagnostics are Rule 3(f)**: "to be used as companion diagnostics". Other relevant items: 3(h) "screening, diagnosis, or staging of cancer"; 3(i) "human genetic testing"; 3(g) disease staging (with life-threatening-management risk); 3(k) management of patients with life-threatening disease; 3(l)/(m) congenital-disorder screening. (So the common statement is right: CDx = Rule 3(f), class C, **not D**.)
- Rule 4 -> self-testing class **C** (exceptions class B: pregnancy, fertility, cholesterol, urine glucose/erythrocytes/leucocytes/bacteria); near-patient testing "classified in their own right".
- Rule 5 -> class **A** (general lab products, instruments, specimen receptacles).
- Rule 6 -> class **B** (default: devices not covered by other rules).
- Rule 7 -> class **B** (controls without assigned values).
- Implementing rules 1.9: if several rules apply, "the rule resulting in the higher classification shall apply".

### 1.6 Annex XIII
- **Part A, Section 1 Performance evaluation**: 1.1 performance evaluation plan (PEP) contents, including "methods, including the appropriate statistical tools" and "potential acceptance criteria"; 1.2 demonstration of scientific validity (1.2.1), analytical performance (1.2.2), clinical performance (1.2.3) - sources incl. literature; clinical performance studies "shall be performed unless due justification is provided"; 1.3 clinical evidence and **performance evaluation report** (1.3.2: includes scientific validity report, analytical performance report, clinical performance report, assessment).
- **Part A, Section 2 Clinical performance studies**: 2.3.2 clinical performance study plan (CPSP) items (a)-(ab), incl. (j) statistical design and bias minimisation, (l) clinical performance parameters and primary/secondary endpoints, (m) population size and representativity, (n) "assurance of relevant method for determining the true clinical status of patient specimens"; 2.3.3 study report. Section 3 other performance studies.
- **Part B Post-market performance follow-up (PMPF)**: Sections 4-8 (PMPF as continuous process, PMPF plan 5.1/5.2, PMPF evaluation report 6, justification if PMPF not appropriate 8). Numbering of Part B continues from Part A (4-8), not restarting at 1.

### 1.7 Medicines-authority consultation for companion diagnostics
Not Art. 47 and not only 48(3)/(4). It is spread across **Art. 48**:
- **48(3)** (class D): "the notified body shall consult a competent authority designated by the Member States in accordance with Directive 2001/83/EC ... or the EMA, as applicable" per Annex IX Section 5.2.
- **48(4)** (class D via Annex X + XI): same consultation, via Annex X Section 3 point (k).
- **48(7)** (class C): "for companion diagnostics the notified body shall for every device follow the procedure for technical documentation assessment laid down in Section 5.2 of Annex IX" and consult the authority/EMA.
- **48(8)** (class C via Annex X + XI): consultation per Annex X Section 3(k).
So the consultee is "a competent authority designated ... in accordance with Directive 2001/83/EC **or the EMA, as applicable**" (national medicines authority OR EMA, depending on the medicinal product's authorisation route). The Annex IX Section 5.2 procedure itself was not read in detail (not verified). Because CDx are class C (Rule 3(f)), the operative paragraphs for typical CDx are 48(7)/(8).

### 1.8 Transitional timeline (as amended) - brief
Verified from amending texts:
- Reg. (EU) 2022/112 (OJ 25 Jan 2022 date of act) introduced staggered legacy-device deadlines (2025/2026/2027) and delayed Art. 5(5) in-house provisions.
- **Reg. (EU) 2024/1860** (adopted 13 June 2024, OJ 9.7.2024, https://eur-lex.europa.eu/eli/reg/2024/1860/oj; also amends the MDR) replaced Art. 110(3) and inserted 110(3a)-(3e):
  - Legacy devices with valid Directive 98/79/EC certificate (3a): may be placed on the market until **31 December 2027** (these certificates "continue to remain valid ... until 31 December 2027", Art. 110(2)).
  - Devices needing a notified body for the first time under IVDR, self-declared under the Directive (3b): **class D 31 Dec 2027; class C 31 Dec 2028; class B and sterile class A 31 Dec 2029**.
  - Conditions (3c): continued compliance with the Directive, no significant design/intended-purpose change, no unacceptable risk, **QMS in place by 26 May 2025**, formal NB application lodged by **26 May 2025 (3a and class D) / 26 May 2026 (class C) / 26 May 2027 (class B/A sterile)**, and written NB agreement signed by **26 Sep 2025 / 26 Sep 2026 / 26 Sep 2027** respectively.
  - Art. 113(3)(j): Art. 5(5)(d) (in-house devices) date changed from 26 May 2028 to **31 December 2030**.
  - Art. 1 point (1) / Art. 2 point (1) of 2024/1860 (Eudamed-related and Art. 10a) apply from 10 Jan 2025; Eudamed obligations now tied to publication-of-notice dates.
- Sell-off/"until" dates in Art. 110(4) and Art. 112 were also rewritten by 2024/1860; I did not extract the final wording (not verified).
- **Pending proposal**: Commission proposal COM(2025) 1023 final, 2025/0404(COD), 16 Dec 2025, "amending Regulations (EU) 2017/745 and (EU) 2017/746 as regards simplifying and reducing the burden of the rules" (opened: https://health.ec.europa.eu/document/download/25e7ea7c-cab3-40cf-86d9-d11f5e7744d8_en?filename=md_com_2025-1023_act_en.pdf). Recital (49) addresses CDx definition and consultation duplication. Legislative status as of Oct 2026 (Council/Parliament positions) came from a web-search summary only: **not verified** from official procedure pages; treat as "proposal, not law".

---

## 2. MDCG 2022-2
- **Title:** "Guidance on general principles of clinical evidence for In Vitro Diagnostic medical devices (IVDs)". **Date: January 2022** (PDF cover; 31 pages). Listed on the Commission MDCG guidance page as "MDCG 2022-2 ... January 2022".
- URL: https://health.ec.europa.eu/document/download/f373538f-939c-472f-9536-436b6ddac085_en
- Status line on cover: endorsed by MDCG (established by Art. 103 of Reg. 2017/745); "not legally binding".
- **Structure (ToC):** 1 Purpose; 2 Scope; 3 Introduction; 4 Definitions; 5 General principles of Clinical Evidence; 6 Performance Evaluation (6.1 process, 6.2 role of risk management, 6.3 Performance Evaluation Plan, 6.4 Scientific Validity, 6.5 Analytical Performance, 6.6 Clinical Performance, 6.7 Clinical performance studies, 6.8 Performance Evaluation Report); 7 Continuous update (7.1 PMS and PMPF); Appendix I Methodological principle for generation of clinical evidence; Appendix II Required frequency for updates of reports.
- Note the ToC lists Appendix II page as 32 on a 31-page document (a typo in the source ToC).
- Takes account of GHTF SG5/N7:2012 concepts (per Section 1).

## 3. ISO 20916:2019
- **Exact title:** "In vitro diagnostic medical devices - Clinical performance studies using specimens from human subjects - Good study practice". Edition 1, published 2019-05, 56 pages, ISO/TC 212; stage 90.93 "International Standard confirmed"; "last reviewed and confirmed in 2025".
- Source opened: https://committee.iso.org/standard/69455.html (the www.iso.org page returned HTTP 403 to my client).
- **Scope (abstract):** "good study practice for the planning, design, conduct, recording and reporting of clinical performance studies ... for regulatory purposes". Excludes: "Analytical performance studies are out of the scope"; studies for non-regulatory purposes such as reimbursement. Lists ISO 14155 as relevant for integrated device systems.
- (Full text paywalled; not read.)

## 4. FDA guidances (all opened at fda.gov guidance pages and PDFs)

| Guidance | Date | Status on FDA page (opened 2026-10-16) | Docket |
|---|---|---|---|
| Statistical Guidance on Reporting Results from Studies Evaluating Diagnostic Tests - Guidance for Industry and FDA Staff | Issued 13 Mar 2007 (draft 12 Mar 2003) | "Final"; page content-current 03/27/2018; no withdrawal notice | FDA-2020-D-0957 |
| In Vitro Companion Diagnostic Devices | Aug 2014 (draft 14 Jul 2011) | "Final"; content-current 09/27/2018 | FDA-2011-D-0215 |
| Principles for Codevelopment of an In Vitro Companion Diagnostic Device with a Therapeutic Product | **Draft, July 2016** (15 Jul 2016) | "Draft"; "Not for implementation"; content-current 09/27/2018; **still draft, not finalised** | FDA-2016-D-1703 |
| Developing and Labeling In vitro Companion Diagnostic Devices for a Specific Group of Oncology Therapeutic Products | **April 2020** | "Final"; Federal Register notice 14 Apr 2020; issued by CBER/CDRH/CDER/OCE | FDA-2018-D-3380 |

URLs: https://www.fda.gov/media/71147/download ; https://www.fda.gov/media/81309/download ; https://www.fda.gov/media/99030/download ; https://www.fda.gov/regulatory-information/search-fda-guidance-documents/developing-and-labeling-vitro-companion-diagnostic-devices-specific-group-oncology-therapeutic

Findings:
- **The 2020 title is "...for a Specific Group of Oncology Therapeutic Products"**. The draft (Dec 2018) was titled "Specific Group or Class"; some FDA pages/secondary sources still say "or Class". Use "Specific Group of".
- None of the four is shown as withdrawn or superseded on the FDA guidance pages I opened. I did not check the FDA's withdrawn-guidance list or newer replacement drafts beyond the listing pages: "no superseding document seen", not a proof of absence.
- **2007 statistical guidance, PPA/NPA claim verified.** Verbatim: "When a new test is evaluated by comparison to a non-reference standard, sensitivity and specificity are not appropriate terms to describe the comparative results." And: "the estimates are called positive percent agreement and negative percent agreement, rather than sensitivity and specificity." Also: "you cannot directly calculate unbiased estimates of sensitivity and specificity." Also warns PPV/NPV likewise not directly estimable, cautions PPA/NPA are asymmetric ("clearly state the calculations being performed"), and "There is no statistical solution" to the non-reference-standard problem; discusses discrepant resolution bias.
- **2014 CDx guidance:** "An IVD companion diagnostic device is an in vitro diagnostic device that provides information that is essential for the safe and effective use of a corresponding therapeutic product." Footnote 10: "most IVD companion diagnostic devices will be Class III devices, although there may be cases when a Class II classification with premarket notification (510(k)) is appropriate." Also: the CDx's use is stipulated in the labeling of both device and therapeutic.
- **2016 draft codevelopment:** opened first page only; status confirmed draft.
- 2020 guidance: only the FDA landing page opened (summary says it describes considerations for development and labeling of CDx for a group of oncology products); the PDF body was not read: details **not verified**.

## 5. FDA pathways and vocabulary (fda.gov pages opened 2026-10-16)
- **510(k) - "clearance":** "a premarket submission made to FDA to demonstrate that the device to be marketed is as safe and effective, that is, substantially equivalent, to a legally marketed device". The device may not be marketed until a substantial-equivalence letter is received. (https://www.fda.gov/medical-devices/premarket-submissions-selecting-and-preparing-correct-submission/premarket-notification-510k)
- **De Novo - "granted":** pathway "for certain new types of devices to obtain marketing authorization as class I or class II devices"; routes: after an NSE determination on a 510(k) (Option 1) or directly (Option 2, no predicate); FDA posts "the granting order"; De Novo devices can serve as predicates. (https://www.fda.gov/medical-devices/premarket-submissions-selecting-and-preparing-correct-submission/de-novo-classification-request)
- **PMA - "approval":** "Premarket approval (PMA) is the FDA process of scientific and regulatory review to evaluate the safety and effectiveness of Class III medical devices"; "The applicant must receive FDA approval of its PMA application prior to marketing". (https://www.fda.gov/medical-devices/premarket-submissions-selecting-and-preparing-correct-submission/premarket-approval-pma)
- **Vocabulary (supported by FDA wording):** Class III -> PMA -> "approved"; Class II -> 510(k) -> "cleared"; De Novo -> "granted" (marketing authorization). FDA's CLIA page itself uses "cleared/approved/licensed/granted". FDA's consumer page https://www.fda.gov/consumers/consumer-updates/it-really-fda-approved says Class III "generally require FDA approval of a premarket approval application" while Class II may market under "510(k) clearance". I did not find a single FDA sentence defining the three verbs side by side; the table above is a synthesis: label it as such.
- **CLIA categorization** (https://www.fda.gov/medical-devices/ivd-regulatory-assistance/clia-categorizations): "waived tests, moderate complexity tests, and high complexity tests"; determined after FDA clears/approves a submission; scored on 7 criteria (1-3 each): "12 or less" moderate, "above 12" high; waived if waived by regulation or cleared/approved for home use; a moderate test may seek a CLIA Waiver by Application. Note this is distinct from the FDA device class (I-III).

## 6. Reporting and quality-assessment tools (PubMed E-utilities record opened; pubmed.ncbi.nlm.nih.gov web pages returned HTTP 203 to my client)
- **STARD 2015:** Bossuyt PM, Reitsma JB, Bruns DE, et al. "STARD 2015: an updated list of essential items for reporting diagnostic accuracy studies." BMJ 2015;351:h5527. doi:10.1136/bmj.h5527. PMID 26511519. Abstract: "an updated list of 30 essential items that should be included in every report of a diagnostic accuracy study". (Parallel publications in Radiology and Clin Chem exist per search results: not opened.)
- **QUADAS-2:** Whiting PF, Rutjes AWS, Westwood ME, et al. "QUADAS-2: a revised tool for the quality assessment of diagnostic accuracy studies." Ann Intern Med 2011;155(8):529-536. doi:10.7326/0003-4819-155-8-201110180-00009. PMID 22007046. Abstract: "This tool comprises 4 domains: patient selection, index test, reference standard, and flow and timing." Risk of bias for all 4; applicability concerns for the first 3; applied in 4 phases.

## 7. ICH E9, E9(R1), CDISC
- **ICH E9:** "Statistical Principles for Clinical Trials", ICH Harmonised Tripartite Guideline, "Current Step 4 version dated 5 February 1998". (https://database.ich.org/sites/default/files/E9_Guideline.pdf, 39 pages)
- **ICH E9(R1):** "Addendum on Estimands and Sensitivity Analysis in Clinical Trials to the Guideline on Statistical Principles for Clinical Trials", "Final version, Adopted on 20 November 2019" (Step 4). (https://database.ich.org/sites/default/files/E9-R1_Step4_Guideline_2019_1203.pdf). Sections include A.3 Estimands, A.3.3 Estimand attributes. These are pharmaceutical-trial guidelines; applicability to diagnostic studies is by analogy (not an IVDR requirement; not verified that any IVD authority mandates them).
- **CDISC:** CDISC publishes device-related standards: **SDTMIG for Medical Devices v1.1 (1 Feb 2019, SDTM v1.7; v1.0 23 Jan 2012)** and **ADaMIG for Medical Devices v1.0 (29 Nov 2021)**. Descriptions: SDTMIG-MD "defines data standards for medical device-related data in clinical research"; ADaMIG-MD addresses "clinical trials in which medical devices are used". (https://www.cdisc.org/standards/foundational/medical-devices). These cover device data in studies generally. **I did not find a CDISC standard specific to IVD/diagnostic-accuracy studies**; a claim of "no IVD-specific CDISC standard" is therefore "none found on the CDISC device page", not proven absence. Whether SDTMIG-MD suits IVD specimen-based studies: not verified.

---

## Corrections to commonly repeated statements
1. Arts 47-48 are classification and conformity assessment, not general safety/performance (that is Annex I / Art. 5).
2. Performance evaluation = Art. 56; Art. 57 = general requirements for performance studies; Art. 58 = additional requirements (interventional, invasive; CDx studies included).
3. CDx consultation of medicines authority/EMA is not only 48(3)/(4): also 48(7) and 48(8) (class C), plus Annex IX 5.2 / Annex X 3(k). Consultee is "a competent authority designated ... under Directive 2001/83/EC or the EMA, as applicable".
4. CDx are class C under Rule 3(f), not class D.
5. FDA 2020 guidance title is "...for a Specific Group of Oncology Therapeutic Products" (final); "Group or Class" was the draft title.
6. Definition numbers: CDx is Art 2(7), not near the performance definitions (36-46).
