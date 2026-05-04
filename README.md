# PhD Retention Analysis
**Ad hoc statistical study conducted for school deans, Claremont Graduate University**

Chi-square test of independence with Bonferroni-corrected pairwise Z-tests on
five years of doctoral enrollment data, identifying a statistically significant
decline in retention and distinguishing real change from normal year-to-year variance.

---

## Overview

This study examined year-to-year retention rates for PhD students in the School
of XXXXXXXXXXXXXXXXX from Fall 2019 through Fall 2023. Retention was
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
| `SES_PHD_Retention_Analysis.ipynb` | Jupyter notebook with Chi-square test and Bonferroni-corrected pairwise Z-tests |

**Note:** The underlying dataset contains student-level enrollment records
and is not included in this repository. Furthermore, the data has been synthetically altered so original aggregate values are masked.

---

## Environment

**Python:** 3.14.4

**Jupyter Components:**

| Component | Version |
|-----------|---------|
| jupyter-core | 5.9.1 |
| jupyter-client | 8.8.0 |
| ipykernel | 7.2.0 |

**Packages:**

```
asttokens               3.0.1
colorama                0.4.6
comm                    0.2.3
contourpy               1.3.3
cycler                  0.12.1
debugpy                 1.8.20
decorator               5.2.1
et-xmlfile              2.0.0
executing               2.2.1
fonttools               4.62.1
ipykernel               7.2.0
ipython                 9.13.0
ipython-pygments-lexers 1.1.1
jedi                    0.20.0
jupyter-client          8.8.0
jupyter-core            5.9.1
kiwisolver              1.5.0
matplotlib              3.10.9
matplotlib-inline       0.2.1
nest-asyncio            1.6.0
numpy                   2.4.4
openpyxl                3.1.5
packaging               26.2
pandas                  3.0.2
parso                   0.8.7
patsy                   1.0.2
pillow                  12.2.0
pip                     26.1
platformdirs            4.9.6
prompt-toolkit          3.0.52
psutil                  7.2.2
pure-eval               0.2.3
pygments                2.20.0
pyparsing               3.3.2
python-dateutil         2.9.0.post0
pyzmq                   27.1.0
scikit-posthocs         0.12.0
scipy                   1.17.1
seaborn                 0.13.2
six                     1.17.0
stack-data              0.6.3
statsmodels             0.14.6
tornado                 6.5.5
traitlets               5.14.3
tzdata                  2026.2
wcwidth                 0.7.0
```
