# Data-to-Decision: Translating Analysis into Policy Insight
##### Author: [Lisa Monozlai](https://www.linkedin.com/in/lisamonozlai/)

This repository demonstrates a structured approach to turning raw data into decision-relevant insight using Python.

The objective is not simply to analyze a dataset, but to illustrate how analytical workflows can inform policy and program prioritization, particularly in environments where resources are limited and tradeoffs matter.

The full analysis is available in three formats, each tailored to a different audience:

- [Jupyter Notebook](https://github.com/lisamonozlai/python-for-public-policy/blob/main/notebook/eda_diabetes_progression.ipynb)  
- [PDF Report](https://github.com/lisamonozlai/python-for-public-policy/blob/main/report/eda_diabetes_progression.pdf)  
- [One‑Page Summary](https://github.com/lisamonozlai/python-for-public-policy/blob/main/summary/eda_diabetes_progression_summary.pdf)

---

## Policy Framing

Effective decisions begin with a clearly defined question:

> **Which factors most influence diabetes progression, and how can that insight guide more effective interventions?**

This framing mirrors real-world program design: before allocating funding or designing interventions, decision-makers must understand which variables exert the greatest influence on outcomes.

---

## Dataset

The analysis uses a 2004 diabetes dataset from the [University of Copenhagen](https://www4.stat.ncsu.edu/%7Eboos/var.select/diabetes.html). It contains standardized clinical and demographic information for 442 individuals and is well-suited for transparent exploratory analysis without extensive preprocessing.

### Demographic Variables
- **age** — Age in years  
- **sex** — Biological sex  

### Body Metrics
- **bmi** — Body mass index  
- **bp** — Average blood pressure  

### Cholesterol and Lipid Measures
- **s1** — Total cholesterol  
- **s2** — LDL cholesterol  
- **s3** — HDL cholesterol  
- **s4** — Total cholesterol-to-HDL ratio  
- **s5** — Triglycerides  
- **s6** — Baseline blood glucose  

### Outcome Variable
- **progression** — Diabetes progression one year after baseline  

---

## Analytical Approach

The workflow follows a structured, decision-oriented sequence:

1. **Data Quality & Distribution Checks**  
   Reviewed distributions to understand scale, spread, and potential anomalies.

2. **Demographic Comparisons**  
   Compared progression across age groups and sex to assess baseline differences.

3. **Clinical Indicator Relationships**  
   Visualized relationships between progression and health metrics using scatter plots.

4. **Relative Strength of Association**  
   Calculated linear trend slopes to compare how strongly each variable relates to progression.

The emphasis is on interpretability and transparency rather than model complexity. In policy environments, clarity often matters more than algorithmic sophistication.

---

## Key Findings

The analysis indicates:

- **Strongest associations:**  
  - Body mass index (BMI)  
  - Triglycerides (s5)

  These variables exhibit the steepest trend slopes, indicating materially stronger relationships with progression than demographic characteristics.

- **Protective relationship:**  
  - HDL cholesterol (s3)

- **Moderate associations:**  
  - Blood pressure  
  - Blood glucose  

- **Limited association:**  
  - Age  
  - Sex  

Notably, the slope magnitude for BMI is substantially larger than that of age, reinforcing that metabolic indicators appear more influential in this dataset than fixed demographic characteristics.

---

## Interpretation

The relative strength of metabolic indicators compared to demographic variables suggests that modifiable risk factors may offer greater intervention leverage than fixed characteristics such as age or sex.

While demographic segmentation can inform outreach strategies, clinical indicators appear more directly associated with measurable progression changes within this sample.

---

## Alignment with Broader Research

These patterns are consistent with established evidence:

- Higher BMI is a known risk factor for type 2 diabetes development and progression ([Nature, 2024](https://www.nature.com/articles/s41598-024-75179-6)).
- Elevated triglycerides are linked to insulin resistance and metabolic dysfunction ([BMC Public Health, 2025](https://pubmed.ncbi.nlm.nih.gov/40165126/); [IJMS, 2025](https://www.mdpi.com/1422-0067/26/20/9910)).

The consistency between exploratory analysis and broader literature strengthens confidence that the observed relationships are directionally meaningful.

---

## Policy Implications

In resource-constrained environments, prioritization is essential.

If designing a program to reduce diabetes progression, this analysis suggests beginning with:

- BMI-focused interventions (nutrition, physical activity, weight management)
- Triglyceride-focused interventions (dietary counseling, lipid management, metabolic health strategies)

The broader takeaway is methodological: structured, transparent analysis can clarify which levers may deliver the highest potential return on intervention effort.

---

## Limitations

This analysis is exploratory and identifies associations rather than causal effects.

The comparison relies on simple linear relationships and does not account for interaction effects, non-linear dynamics, or longitudinal variation beyond the one-year progression measure.

Findings should therefore inform prioritization discussions rather than replace deeper clinical modeling or randomized evaluation.

---

## Why This Project Matters

This repository demonstrates how Python can:

- Convert raw data into interpretable insight  
- Support evidence-informed decision-making  
- Provide a transparent, reproducible workflow  
- Communicate findings across technical and non-technical audiences  

The same analytical framework can be adapted to other policy, program, or operational questions where decision-makers must determine which factors matter most.

---

## License

MIT
