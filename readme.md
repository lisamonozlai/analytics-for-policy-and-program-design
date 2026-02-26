# Using Python to Support Policy Decision‑Making
##### Author: [Lisa Monozlai](https://www.linkedin.com/in/lisamonozlai/)

This project demonstrates how Python can support policy and program decision‑making by turning raw data into clear, interpretable insights. The analysis is available in three formats, each tailored to different audiences (technical, working‑level, and executive):

- [Jupyter Notebook](https://github.com/lisamonozlai/python-for-public-policy/blob/main/notebook/eda_diabetes_progression.ipynb)  
- [PDF Report](https://github.com/lisamonozlai/python-for-public-policy/blob/main/report/eda_diabetes_progression.pdf)  
- [One‑Page Brief](https://github.com/lisamonozlai/python-for-public-policy/blob/main/summary/eda_diabetes_progression_summary.pdf)

## Dataset
To demonstrate a data‑to‑decision workflow, I use a 2004 diabetes dataset (`diabetes.csv`) from the [University of Copenhagen](https://www4.stat.ncsu.edu/%7Eboos/var.select/diabetes.html). It includes standardized clinical and demographic information for 442 individuals.

**Demographic variables**

age — Age in years.

sex — Biological sex (male or female).

**Body metrics**

bmi — Body mass index, an indicator of body fat and metabolic risk.

bp — Average blood pressure, related to heart and metabolic health.

**Cholesterol and lipid measures**

s1 — Total cholesterol.

s2 — Low-density lipoprotein (LDL, “bad” cholesterol).

s3 — High-density lipoprotein (HDL, “good” cholesterol).

s4 — Total cholesterol-to-HDL ratio.

s5 — Triglycerides, often linked to insulin resistance.

**Blood glucose**

s6 — Baseline blood glucose level.

**Outcome variable**

Progression — Diabetes progression one year after baseline, used to assess how initial health measures relate to disease change over time.

## Goals
The analysis aims to identify which factors most influence diabetes progression so public health teams can focus their programs and interventions where they will have the greatest impact.

## What I Did
- Checked data quality and distributions  
- Compared progression across age and sex groups  
- Visualized relationships between health indicators and progression  
- Used simple trend lines to compare the strength of relationships  

## What I Found
- **Strongest influence:** body mass index (BMI) and triglycerides  
- **Protective effect:** HDL (“good”) cholesterol  
- **Moderate influence:** blood pressure and blood glucose  
- **Limited influence:** age and sex  

These results align with medical expectations and highlight which factors may matter most.

## Other Research
These findings are consistent with broader evidence:  
- Studies show that people with increasing BMI are more likely to develop diabetes ([Nature, 2024](https://www.nature.com/articles/s41598-024-75179-6)).  
- Elevated triglycerides are linked to insulin resistance, which contributes to faster progression ([BMC Public Health, 2025](https://pubmed.ncbi.nlm.nih.gov/40165126/); [IJMS, 2025](https://www.mdpi.com/1422-0067/26/20/9910)).

## Policy Conclusions
If designing a program to reduce diabetes progression, it may be most effective to prioritize interventions targeting BMI and triglycerides, as these factors show the strongest influence in both the analysis and the broader research literature.

## License
MIT
