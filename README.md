# Nonparametric Statistics Project — Maternal Factors and Child IQ

**Course:** Nonparametric Statistics
**Team:** Constantin Teodor-Vasile, Erhan Teodora-Miruna, Dumitrescu Andrei
**Group:** 1067, Series F — ASE Bucharest, ASDS Master's Program

**File:** `Proiect_statistica_neparametrica_final.docx`

---

## Overview

This project investigates which maternal factors influence a child's cognitive performance, measured by the PPVT (Peabody Picture Vocabulary Test) score. All analysis was conducted in SPSS using nonparametric statistical methods.

## Research Questions

1. Is there a relationship between child IQ and the mother's age?
2. To what extent does the mother's level of education influence child IQ?
3. Are there significant IQ differences between children of mothers with at most a high school diploma vs. those with university-level education?
4. Are there significant IQ differences across three maternal education groups?
5. Does the distribution of child IQ scores follow a normal distribution?
6. What are the overall factors that influence child intelligence?

## Dataset

| Variable | Type | Description |
|---|---|---|
| `testscore` | Quantitative | Child's PPVT score |
| `education` | Ordinal (1–4) | 1 = No high school · 2 = High school graduate · 3 = Some college · 4 = College graduate |
| `momage` | Quantitative | Mother's age at birth |
| `grupMann` | Binary grouping | Derived from `education` for Mann-Whitney test |
| `grupKruskal` | 3-group | Derived from `education` for Kruskal-Wallis test |
| `binar` | Binary | Derived from `education` for point-biserial correlation |

## Methods & Results

| Method | Variables | Result |
|---|---|---|
| Pearson correlation | `testscore` × `momage` | Weak positive (r = 0.111, p = 0.027) — statistically significant |
| Kendall & Spearman correlation | `binar` × `testscore` | Weak positive (τ = 0.111, ρ = 0.135), both p < 0.01 |
| Mann-Whitney test | 2 education groups × `testscore` | No significant difference (p = 0.071 > 0.05) |
| Kruskal-Wallis test | 3 education groups × `testscore` | Significant differences found (p < 0.01) |
| Shapiro-Wilk test | `testscore` | Normality assessment of the IQ score distribution |

## Conclusions

- Older mothers tend to have children with slightly higher IQ scores, but the effect is weak.
- Having a college degree is positively (but weakly) associated with higher child IQ.
- When split into only 2 groups (≤ high school vs. college), differences are not statistically significant.
- When split into 3 groups, significant differences emerge across education levels.

## Software

SPSS (all nonparametric tests and correlation coefficients)
