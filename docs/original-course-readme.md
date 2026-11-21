# AMOD 5240H Statistical Analysis Project

> **Language / 语言 / Ngôn ngữ:** [English](README.md) | [中文](README.zh.md) | [Tiếng Việt](README.vi.md)

## Course Information

- **Course:** AMOD 5240H - Applied Statistics
- **Instructor:** Dave Riegert
- **Term:** Winter 2026

## Team Members

- Feng Qiu
- Keyao Li
- Ngoc Vy

## Project Overview

This project applies statistical methods covered in AMOD 5240H to analyze a real-world dataset. The analysis includes exploratory data analysis (EDA), linear regression modeling, and hypothesis testing to investigate factors affecting student academic performance in secondary education.

## Dataset

**Name:** Student Performance Dataset

**Source:** [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/320/student+performance)

**File:** `student-por.csv` (Portuguese language course)

**Instances:** 649 students

**Features:** 33 variables (30 predictors + 3 grade variables)

### Description

This dataset contains student achievement data from two Portuguese secondary schools (Gabriel Pereira and Mousinho da Silveira). The data was collected through school reports and student questionnaires, capturing demographic, social, and behavioral information alongside academic performance.

### Variables

#### Target Variables (Grades)
| Variable | Description | Range |
|----------|-------------|-------|
| G1 | First period grade | 0-20 |
| G2 | Second period grade | 0-20 |
| G3 | Final grade (primary target) | 0-20 |

#### Demographic Attributes
| Variable | Description | Type |
|----------|-------------|------|
| school | Student's school (GP or MS) | Binary |
| sex | Student's sex (F/M) | Binary |
| age | Student's age | Numeric (15-22) |
| address | Home address type (U: Urban, R: Rural) | Binary |
| famsize | Family size (LE3: ≤3, GT3: >3) | Binary |
| Pstatus | Parent's cohabitation status (T: Together, A: Apart) | Binary |

#### Parental Information
| Variable | Description | Type |
|----------|-------------|------|
| Medu | Mother's education (0-4) | Ordinal |
| Fedu | Father's education (0-4) | Ordinal |
| Mjob | Mother's job | Nominal |
| Fjob | Father's job | Nominal |

#### School-Related Features
| Variable | Description | Type |
|----------|-------------|------|
| reason | Reason to choose this school | Nominal |
| guardian | Student's guardian | Nominal |
| traveltime | Home to school travel time (1-4) | Ordinal |
| studytime | Weekly study time (1-4) | Ordinal |
| failures | Number of past class failures | Numeric |
| schoolsup | Extra educational support | Binary |
| famsup | Family educational support | Binary |
| paid | Extra paid classes | Binary |
| activities | Extra-curricular activities | Binary |
| nursery | Attended nursery school | Binary |
| higher | Wants to take higher education | Binary |
| internet | Internet access at home | Binary |

#### Social/Behavioral Factors
| Variable | Description | Type |
|----------|-------------|------|
| romantic | In a romantic relationship | Binary |
| famrel | Quality of family relationships (1-5) | Ordinal |
| freetime | Free time after school (1-5) | Ordinal |
| goout | Going out with friends (1-5) | Ordinal |
| Dalc | Workday alcohol consumption (1-5) | Ordinal |
| Walc | Weekend alcohol consumption (1-5) | Ordinal |
| health | Current health status (1-5) | Ordinal |
| absences | Number of school absences | Numeric (0-93) |

## Variable Assignments

| Member | Variable |
|--------|----------|
| Feng Qiu | `reason` |
| Ngoc Vy | `failures` |
| Keyao Li | `address` |

## Project Progress

| Component | Due Date | Weight | Status |
|-----------|----------|--------|--------|
| Part 1: Data Background and Variables | February 13, 2026 | 4% | Completed |
| Part 2: EDA and Analysis Proposal | March 6, 2026 | 4% | Completed |
| Presentation | April 3, 2026 | 4% | Completed |
| Part 3: Final Report | April 10, 2026 | 8% | Completed |

---

### Part 1 — Data Background and Variables ✅

- [x] Dataset introduction
- [x] Variable descriptions
- [x] Research context (suitability for linear regression)
- [x] Data quality considerations (missing values, outliers, cleaning)

---

### Part 2 — EDA and Analysis Proposal ✅

#### EDA
- [x] `reason` (Feng Qiu)
- [x] `failures` (Ngoc Vy)
- [x] `address` (Keyao Li)

#### Written Sections
- [x] 2.1 Brief Dataset Reminder
- [x] 2.3 Research Questions (linear regression + one-way ANOVA)
- [x] 2.4 Proposed Analysis Plan
- [x] 2.5 Potential Challenges
- [x] Appendix containing Part 1

---

### Part 3 — Final Report [~8–12 pages] — Due April 10, 2026

#### Content Tasks

- [x] **Executive Summary** — all three predictors covered (`reason`, `failures`, `address`) ✅
- [x] Introduction and Background (refined Part 1) ← Feng ✅
- [x] Exploratory Data Analysis
  - [x] `reason` EDA ← Feng ✅
  - [x] `failures` EDA ← Vy ✅
  - [x] `address` EDA ← Keyao ✅
- [x] Methodology
  - [x] Methodology overview and statistical framework ← Vy ✅
  - [x] SLR: G3 ~ `reason` (equation, F-test, t-tests, 95% CIs) ← Feng ✅
  - [x] SLR: G3 ~ `failures` (equation, F-test, t-tests) ← Vy ✅
  - [x] SLR: G3 ~ `address` (equation, F-test, 95% CIs) ← Keyao ✅
  - [x] Linear regression assumptions stated and verified ← Feng ✅
- [x] Results
  - [x] One-way ANOVA: G3 by `reason` (F-stat, Levene's, Tukey HSD) ← Feng ✅
  - [x] One-way ANOVA: G3 by `failures` (F-stat, Tukey HSD) ← Vy ✅
  - [x] Two-sample t-test: G3 by `address` ← Keyao ✅
  - [x] Diagnostic plots for `reason` model (Residuals vs Fitted, Scale-Location, Q-Q) ← Feng ✅
  - [x] Diagnostic plots for `failures` model ← Vy ✅
  - [x] Decision on G3 = 0 cases — excluded and documented ← Feng ✅
- [x] Discussion
  - [x] `reason` results discussed ← Feng ✅
  - [x] `address` results discussed ← Keyao ✅
  - [x] `failures` results discussed ← Vy ✅
  - [x] Model assumptions verified ← Feng ✅
  - [x] Limitations documented ← Feng ✅
- [x] **Conclusion** — Section 5 added (5.1 Key Findings, 5.2 Implications, 5.3 Remaining Questions) ✅

#### Format / Compliance Fixes

- [x] **Executive Summary** — all three predictors added ✅
- [x] **Conclusion** — `## 5. Conclusion` added ✅
- [x] **Group number** added to title page (Group 6) ✅
- [x] **Code hidden / Appendix added** — global `execute: echo: false` in YAML; all 44 chunks labeled; `\newpage` + `# Appendix: Full R Code` section added with `ref-label: !expr knitr::all_labels()` ✅
- [x] **Section numbering in Part 1** — Sections 1.5, 1.6, 1.7 renumbered as 1.4.1, 1.4.2, 1.4.3; cross-reference in Section 1.4.3 updated ✅

---

### Presentation ✅ — Completed April 3, 2026

## Key Findings (EDA)

### `reason` — Reason for Choosing School
| Reason | n | Mean G3 | SD |
|--------|---|---------|----|
| reputation | 143 | 12.94 | 3.05 |
| home | 149 | 12.18 | 2.95 |
| course | 285 | 11.55 | 3.11 |
| other | 72 | 10.69 | 3.93 |

Students who chose the school for its reputation achieved the highest mean final grade. The "other" group showed the most variability. SLR: F(3, 630) = 10.5, p ≈ 0, R² = 4.8%. Tukey HSD: reputation vs. course and reputation vs. other are the only significant pairs.

### `failures` — Past Class Failures
| Failures | n | Mean G3 |
|----------|---|---------|
| 0 | 549 | 12.51 |
| 1 | 70 | 8.64 |
| 2 | 16 | 8.81 |
| 3 | 14 | 8.07 |

A single past failure is associated with a sharp drop in final grades (~4 points). The effect does not appear to be cumulative across 1–3 failures.

### `address` — Home Address Type
| Address | n | Mean G3 |
|---------|---|---------|
| Urban (U) | 452 | 12.3 |
| Rural (R) | 197 | 11.1 |

Urban students outperform rural students by ~1.2 points on average. Zero-grade cases are spread across both groups (11 urban, 4 rural). Urban students also show a higher median and a more concentrated IQR.

## Repository Structure

```
5240-project/
├── README.md                        # Project documentation (English)
├── README.zh.md                     # Project documentation (Chinese)
├── README.vi.md                     # Project documentation (Vietnamese)
├── 5240H Project.qmd                # Main Quarto analysis document
├── 5240H-Project.pdf                # Rendered report
├── student-por.csv                  # Dataset (Portuguese course)
├── references.bib                   # Bibliography
├── apa.csl                          # APA citation style
├── presentation/                    # Presentation materials
│   ├── Is Your GPA Your Fault?.key  # Keynote slides
│   ├── 2015_TrentU PPT Template_FINAL2.potx
│   ├── presentation outline.md      # Slide-by-slide outline (English)
│   ├── presentation outline.zh.md   # Slide-by-slide outline (Chinese)
│   └── presentation outline.vi.md   # Slide-by-slide outline (Vietnamese)
└── docs/                            # Reference documents
    ├── 5240-project-part0_overview-wi26.pdf
    ├── 5240-project-part1_background-wi26.pdf
    ├── Standard Operating Procedure_ Variable Screening.pdf
    ├── Project Revised.pdf
    └── How to Merge Main into Your Personal Branch via GitHub Desktop.md
```

## Tools

- **R** for statistical analysis
- **Quarto** for document rendering
- **ggplot2** / **tidyverse** for visualization and data wrangling

## License

The dataset is licensed under [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).

## References

Cortez, P., & Silva, A. (2008). Using data mining to predict secondary school student performance. In *Proceedings of 5th Annual Future Business Technology Conference* (pp. 5-12). EUROSIS.

UCI Machine Learning Repository. (2014). Student Performance Dataset. https://archive.ics.uci.edu/dataset/320/student+performance

OECD. (2012). *Equity and quality in education: Supporting disadvantaged students and schools*. OECD Publishing.
