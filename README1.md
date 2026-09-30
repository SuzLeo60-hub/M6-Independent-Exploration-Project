# 2026 QS World University Rankings Data Analysis

## Overview of the Dataset
- **Source:** QS World University Rankings 2026 (official data derived from QS Quacquarelli Symonds)  
- **Size:** 1,501 institutions, 30 variables  
- **Coverage:** Universities worldwide, with metrics for academic reputation, employer reputation, faculty/student ratio, internationalization, sustainability, and overall performance  
- **Structure:**
  - **Categorical:** Institution name, country, region, size, focus, status  
  - **Numerical:** AR SCORE, ER SCORE, ISR SCORE, IRN SCORE, SUS SCORE, etc.  

---

## Data Cleaning Steps
- **Missing Values:**  
  - Numeric fields (e.g., AR SCORE, ER SCORE) → filled with **median** to avoid bias from extreme outliers.  
  - Categorical fields (e.g., Region, Status) → filled with **mode** to maintain the most frequent institutional attributes.  
- **Duplicates:** Checked and confirmed none.  
- **Outliers:** Identified but **not removed**, since the outliers represent real performance differences (elite universities vs. lower performers). Removing them would distort the reality of global rankings.

---

## Analysis Steps
1. Data exploration (shape, datatypes, missing values).  
2. Data cleaning (median/mode imputation, verify uniqueness).  
3. Statistical analysis of key metrics (mean, standard deviation, distributions).  
4. Visualization of trends and relationships (e.g., ISR vs Overall Score, IRN vs Overall Score).  
5. Benchmarking top performers (MIT, Imperial College, Oxford, Toronto).  
6. Generating actionable insights and recommendations for institutions and policymakers.  

---

##  Key Conclusions
- **Prestige matters most:** Academic and employer reputation are the strongest predictors of overall scores.  
- **Sustainability is rising:** With a mean score of 51, it’s becoming a baseline expectation.  
- **Internationalization varies:** High ISR or IRN does not guarantee high overall performance—academic strength remains primary.  
- **Clustering effect:** Many universities are grouped around an overall score of ~40, suggesting banded rankings.  
- **Regional trends:** US and UK dominate the top, but Asia is quickly gaining ground, especially in research collaboration.

---

## Recommendations
- **For universities:**  
  - Strengthen academic reputation through research visibility and faculty excellence.  
  - Build and develop stronger employer engagement pipelines to improve employability outcomes.  
  - Use international student and faculty diversity as a strategic differentiator, not the sole driver.  

- **For policymakers:**  
  - Support international collaborations and research consortia.  
  - Incentivize sustainability initiatives to continue their positive trend.  

---

## 📂 Project Structure
- `data/` – dataset files  
- `notebooks/` – Jupyter notebooks with analysis and visualizations  
- `presentation/` – PowerPoint summary of findings  
- `README.md` – Project Overview  

---

## 🚀 Next Steps
- Run regression/correlation modeling to quantify factor influence on overall scores.  
- Benchmark universities by region and create strategic improvement playbooks.  
- Refine visualizations with regression lines and annotations for clearer storytelling.  
