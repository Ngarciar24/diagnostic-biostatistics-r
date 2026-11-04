**[S]** = verified in a primary public source (2026-10-16); **[Y]** = synthesis. "NV" = not verified: paywalled.

## Document map (CLSI editions verified on clsi.org)

| Question | Document |
|---|---|
| Precision | **EP05 Ed4 (2025-12)**; A3 (2014): 20 days × 2 runs × 2 reps |
| Verify precision/bias | EP15-A3 (2014): ≤5 working days; bias ≥25 results over ≥5 days |
| LoB/LoD/LoQ | EP17-A2 (2012) |
| Linearity | EP06 Ed2 (2020) |
| Method comparison | EP09c Ed3 (2018) |
| Interference | EP07 Ed3 (2018); EP37 tables |
| Stability / lots | **EP25 Ed2 (2023)**; **EP26 Ed2 (2022)** |
| Binary tests | EP12 Ed3 (2023) |
| ROC | EP24-A2 (2011) |
| Reference intervals | EP28-A3c (2010) |
| Framework | **EP19 Ed3 (2022)**; specimen types **EP35 Ed2 (2025)** |

Design counts for most EP documents: NV.

## Formulas

| Topic | Formula |
|---|---|
| Within-lab SD | √(σ²day + σ²run + σ²rep); CV% = 100·SD/mean [Y] |
| Satterthwaite df | (Σ cᵢMSᵢ)² / Σ (cᵢMSᵢ)²/dfᵢ; 20×2×2 ≈ 70 df |
| UVL | claim·√(χ²₀.₉₅,ν/ν) [Y] |
| LoB / LoD | mean_b + 1.645 SD_b; LoB + 1.645 SD_low |
| Probit LoD95 | 10^((1.645 − b₀)/b₁) |
| Bias at Xc | a + (b − 1)·Xc |
| Total error | \|bias\| + 1.96 SD |
| PPV | Se·p / (Se·p + (1−Sp)(1−p)) |
| LR+ / LR− | Se/(1−Sp); (1−Se)/Sp |
| Wilson CI | (p̂ + z²/2n ± z√(p̂q̂/n + z²/4n²)) / (1 + z²/n) |
| n cases (Se ± d) | z²p(1−p)/d²; total = cases/prevalence |
| AUC | P(case > control); DeLong var from structural components |
| RCV | exp(± 1.96 √2 SD_w) − 1 |
| Deming slope | (s_yy − δs_xx + √((s_yy − δs_xx)² + 4δs_xy²)) / 2s_xy |

## Regulatory anchors

| Item | Fact |
|---|---|
| IVDR Art 47 / 48 | classification / conformity assessment |
| Art 56 / 57 / 58 | performance evaluation / study requirements / additional (58(2) CDx) |
| Annex I 9.1(a)(b) | analytical / clinical parameters |
| Annex VIII | **Rule 3(f): CDx = class C** |
| Art 48(7)(8) | CDx: consult competent authority (2001/83/EC) or EMA |
| Annex XIII | Part A PEP, PER, CPSP 2.3.2; Part B PMPF |
| Art 2(7)(38)(40)(41) | CDx; scientific validity of analyte; analytical; clinical performance |
| Transition 2024/1860 | legacy to 31 Dec 2027; D 2027, C 2028, B 2029 |
| MDCG 2022-2 | clinical evidence for IVDs (Jan 2022) |
| ISO 20916:2019 | clinical performance studies, good study practice |
| 510(k) / De Novo / PMA | cleared / granted / approved [Y] |
| FDA 2007 | PPA/NPA, not Se/Sp, vs non-reference |
| FDA CDx | 2014 final; 2016 codevelopment **draft**; 2020 "Specific Group of Oncology…" final |
| STARD / QUADAS-2 | 30 items / 4 domains |
| ICH E9, E9(R1) | 1998, 2019 (by analogy) |
| CDISC | SDTMIG-MD v1.1, ADaMIG-MD v1.0; no IVD standard found |

## Elecsys pTau217 (FDA K261686, decision 2026-08-19)

| Item | Fact |
|---|---|
| Cut-offs pg/mL | neg ≤ 0.223; int > 0.223–≤ 0.378; pos > 0.378 |
| Pivotal | N 958; PET+ 378 (39.5%); 6-reader visual read |
| 3×2 (PET+/PET−) | pos 285/37; int 72/119; neg 21/424 |
| Headline | PV pos 88.5%; NPV 95.3%; intermediate 19.9%; PPA 75.4%; NPA 73.1% |
| Not in summary | eGFR analysis; monitoring exclusion (Roche release only) |
| Papers | prototype assay; Hibar 0.189 single cut-off; Hortsch 5.78% indeterminate |

## Rules of thumb [Y]

- Se/Sp need a reference standard; otherwise PPA/NPA.
- Lock cut-offs before validation; fix the ≤ / < convention.
- Intermediates: report fraction, per-category PV, PPA/NPA with intermediates as misses.
- Missing bridging samples: ask why; MI needs arm × outcome term; tipping-point.
- Non-significant ≠ equivalent: use CI inside the limit.
- Treat NV items as unverified; do not state them as fact.
