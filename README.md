# PhD Retention Analysis
**Ad hoc statistical study conducted for school deans, Claremont Graduate University**

Chi-square test of independence with Bonferroni-corrected pairwise Z-tests on
five years of doctoral enrollment data, identifying a statistically significant
decline in retention and distinguishing real change from normal year-to-year variance.

---

## Overview

This study examined year-to-year retention rates for PhD students in the School
of Educational Studies (SES) from Fall 2019 through Fall 2023. Retention was
defined as a student remaining enrolled or having graduated (with an MA or PhD)
in the following Fall term.

The goal was to determine whether observed changes in retention rates across
years represented statistically significant shifts or normal variation — and to
provide school leadership with a defensible basis for any policy response.

---

## Methods

**Step 1 — Chi-square test of independence**
A Chi-square test was run on the full contingency table (year × retained/not
retained) to determine whether any significant difference existed across the
five-year period.

- Result: statistically significant (p = 0.0064, df = 4) — at least one pair
  of years showed a meaningful change

**Step 2 — Pairwise proportion Z-tests with Bonferroni correction**
Pairwise two-proportion Z-tests were conducted across all year combinations.
Bonferroni correction was applied to control for the family-wise error rate
across multiple comparisons.

- Result: a statistically significant **decrease of 20.0%** in retention was
  found between Fall 2019 and Fall 2021 (p = 0.0121 after correction)
- All other year-to-year differences were not significant — consistent with
  normal variance in enrollment and graduation patterns

---

## Key Finding

> A statistically significant 20% decline in PhD retention occurred between
> Fall 2019 and Fall 2021. Changes in other years were not significant and
> are best explained by normal variation.

---

## Repository Contents

| File | Description |
|------|-------------|
| `retention_analysis.R` | R code for Chi-square test and Bonferroni-corrected pairwise Z-tests |

**Note:** The underlying dataset contains student-level enrollment records
and is not included in this repository.

---

## Tools & Packages

- **R** — `dplyr`, `stats`
- Chi-square: `chisq.test()`
- Pairwise proportions: `pairwise.prop.test()` with Bonferroni adjustment
