# Diagnostic biostatistics in R

[![render-and-test](https://github.com/Ngarciar24/diagnostic-biostatistics-r/actions/workflows/book.yml/badge.svg)](https://github.com/Ngarciar24/diagnostic-biostatistics-r/actions/workflows/book.yml)

The statistics of in-vitro diagnostics, worked in R on simulated data: analytical performance, diagnostic accuracy and cut-offs, sample size, companion-diagnostic bridging, and a statistical analysis plan with a dry run and an independent re-derivation.

**Read it as a book:** <https://ngarciar24.github.io/diagnostic-biostatistics-r/> · two-page [reference card (PDF)](reference-card.pdf)

## Contents

| Chapter | Topic | Governing documents |
|---|---|---|
| 1 | [Landscape and vocabulary](chapters/01-landscape.qmd) | IVDR, MDCG 2022-2, ISO 20916, FDA pathways |
| 2 | [Precision and variance components](chapters/02-precision.qmd) | CLSI EP05, EP15 |
| 3 | [Detection capability and linearity](chapters/03-detection-linearity.qmd) | EP17, EP06 |
| 4 | [Method comparison, interference, stability, lots](chapters/04-method-comparison.qmd) | EP09c, EP07, EP25, EP26 |
| 5 | [Diagnostic accuracy, ROC](chapters/05-diagnostic-accuracy.qmd) | EP12, EP24, FDA 2007 guidance, STARD |
| 6 | [Cut-offs, two-cut-off designs, intermediate zone](chapters/06-cutoffs.qmd) | EP24, EP12, FDA decision summary K261686 |
| 7 | [Sample size and power](chapters/07-sample-size.qmd) | Buderer, Flahault, Hanley–McNeil |
| 8 | [Companion diagnostics and bridging](chapters/08-companion-diagnostics.qmd) | FDA CDx guidances, IVDR Art 48 |
| 9 | [Statistical analysis plan](chapters/09-sap.qmd) | IVDR Annex XIII, ISO 20916, ICH E9 |
| 10 | [Reference intervals and longitudinal biomarkers](chapters/10-reference-longitudinal.qmd) | EP28 |

Each chapter has four parts: the concept, its regulatory anchor, an R lab with at least one independent cross-check (a second package, a hand formula or a simulation), and the claims it rests on.

## Highlights

- **A mock SAP with a dry run** ([`mock_sap/sap_ptau217_mock.qmd`](mock_sap/sap_ptau217_mock.qmd)): a two-cut-off plasma biomarker against amyloid PET, with co-primary endpoints, performance goals, exact sample size, rules for invalid and intermediate results, subgroups and table shells filled with simulated results. An independent re-derivation reproduced the primary endpoints after it exposed a boundary-convention bug in the lead code.
- **Cut-offs that are locked, then validated** (Chapter 6): derivation and validation cohorts, three implementations cross-checked, and how prevalence and kidney function move the intermediate zone.
- **Bridging a clinical-trial assay to the final companion diagnostic** (Chapter 8): PPA/NPA against a comparator, efficacy in the CDx-positive population when bridging samples are missing, multiple imputation and a tipping-point analysis.
- **Analytical studies** (Chapters 2–4): EP05-style variance components three ways (ANOVA, mixed model, Bayesian), parametric, non-parametric, probit and bootstrap limits of detection, Deming and Passing–Bablok regression.

## How it was made

Written with Claude Code as an AI-assisted coding workflow. Every claim carries its source, the date it was checked and a confidence level in [`claims_ledger.csv`](claims_ledger.csv); the K261686 figures were re-checked by hand against the FDA decision-summary PDF. Known limits are listed below.

## Run it

```r
renv::restore()                          # pinned package versions (R 4.3.3); limma comes from Bioconductor
testthat::test_dir("tests/testthat")     # unit tests of the helper functions
```

```sh
quarto render                            # the book, into _book/
quarto render cheatsheet_pdf/cheatsheet.qmd && cp cheatsheet_pdf/cheatsheet.pdf reference-card.pdf
Rscript mock_sap/simulate_study.R        # only if you change the simulated study
```

Requires Quarto ≥ 1.6 and R ≥ 4.3. Chapter 2 reads cached posterior draws from `cache/`; delete them to refit the Stan model (about 2 minutes, needs a C++ toolchain). GitHub Actions runs the tests, renders the book and publishes it on every push to `main`.

## Known limits

- CLSI design counts for most documents (EP05 Ed4, EP17, EP06, EP09c, EP12, EP28) are **not verified: paywalled**. The chapters use simulation sizes of their own and say so.
- Web sources were read through a fetch tool that summarises pages; key items were re-checked by hand (K261686), but CLSI edition pages and several regulatory facts were not independently re-opened. Re-check in a browser before quoting in regulated material.
- Statements marked [Y] (for example the cleared/granted/approved verb mapping, the EP15 verification-limit formula, the R-environment practices) are synthesis, not quotations.
- The SAP and all study data are simulated teaching material, not an accepted regulatory template.
- The FDA 510(k) database page and the product labelling were not accessible; K261686 data come from the decision-summary PDF (and openFDA for dates).

## Layout

```
index.qmd, chapters/        the book
mock_sap/                   SAP template, the filled mock SAP, its simulation and data
R/helpers.R, R/bridging.R   shared functions, unit-tested in tests/testthat/
cache/                      cached posterior draws and a reference-interval fit
claims_ledger.csv           every claim with source, date and confidence
research/                   source notes and ledgers by topic (CLSI, regulatory, pTau217)
question_map.csv            analysis question → governing document → R tools
cheatsheet_body.md          the reference card; cheatsheet_pdf/ builds the PDF
```
