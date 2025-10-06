
# Product Weight Optimisation to Reduce Giveaway: Causal Inference and Advanced Analytics

## Project Overview: The Give-Away Challenge

This project focuses on leveraging **Causal Inference Analysis, Combinatorial** and **Advanced Analytics** to systematically reduce product "giveaway" (overfilling) in a high-volume soft cheese manufacturing process. At the start of the project, weight variation in the target soft cheese product led to an annual giveaway costing the business significant six-figure losses.

Traditional quality control methods failed to identify the precise causes of weight variation due to the complex interaction of mechanical, process, and biological variables. This work introduced a data-driven, experimental approach to:

1.  **Identify Causal Factors:** Determine which operational settings (e.g., automated equipment settings, operator intervention) had the most significant causal impact on the final product weight variation.
2.  **Quantify Errors:** Develop a predictive model to quantify the contribution of each factor to the final weight error, providing a foundation for automated control.

The project successfully reduced the average giveaway from **21% to 9%** through data-driven operational improvements, with further implementation and scaling across other products leading to cost savings exceeding **£600,000 per annum** through planned automation.

---

## Methodology: Experimentation and Two-Part Analysis

The solution was achieved by combining controlled manufacturing experiments to generate high-quality data, with a two-part analytical approach (EDA and Machine Learning) to deduce patterns and quantify causes / effects.

### 1. Equivalence Class Experiments (EC)

A series of controlled experiments were designed and executed on the manufacturing floor. These "Equivalence Class Experiments" were crucial for creating high-quality, targeted datasets. The experiments systematically varied key operational practices, such as the number of curd tipping scrapes and the automated filling equipment (AFE) settings, allowing for a **causal inference** approach to analysis.

### 2. Analytical Workflow

The project analysis was executed in two distinct stages (corresponding to the two Jupyter notebooks):

| Stage | Focus & Goal | Notebook | Key Techniques |
| :--- | :--- | :--- | :--- |
| **Part 1: Causal Inference & EDA** | **Identification:** Use descriptive and statistical methods to identify and visualise the correlation between experimental variations and weight error. This stage established the **potential causal relationships**. | `part_1_sc_weight_error_analysis_eda.ipynb` | Descriptive Analytics, Statistical Testing, Data Visualisation (e.g., box plots by tray position). |
| **Part 2: Predictive Modelling** | **Validation & Quantification:** Apply Machine Learning (ML) to validate the causal findings from Part 1 and to quantify the contribution of each variable in predicting the **'cheese weight error'** target variable. | `part_2_sc_weight_error_analysis_ml_model.ipynb` | Regression Models (Random Forest, XGBoost), Feature Importance (Permutation Importance), Model Validation. |

---

## Technical Implementation

The analysis was implemented entirely in the Python environment, focusing on transparency and replicability of the findings.

### Key Tools and Libraries

| Category | Tool / Library | Purpose |
| :--- | :--- | :--- |
| **Model** | Scikit-learn (Random Forest, XGBoost) | Predictive model development to validate feature importance. |
| **Data Handling** | Pandas, NumPy | Data ingestion, cleaning, and engineering of experimental features. |
| **Visualisation** | Matplotlib, Seaborn, | Exploratory Data Analysis (EDA) and presentation of causal effects. |
| **Environment** | Jupyter Notebook (Python) | Code execution and step-by-step reporting of analysis. |

### Key Findings

The combination of controlled experimentation and analytical modelling identified and quantified the effects of several key factors responsible for the weight variation, including:
* **AFE Height Setting:** The primary mechanical driver of the mean weight.
* **Curd Tipping Scrape Count:** Operator influence causing significant variation.
* **Tray Position (Inner/Outer):** The location of the cheese within the tray stack, influencing moisture and weight.

**Before (Fig 1):** Initial weight distribution prior to project:

<img width="733" height="514" alt="Screenshot 2025-10-07 at 00 32 33" src="https://github.com/user-attachments/assets/ac6399ef-fff7-42ef-a5b1-c8f79442f02f" />



**After (Fig 2):** By implementing automated AFE filling machine adjustments informed by experimentation and analysis, a flatter weight distribution and reduced inter-tray variation was obtained. Compare Fig 1:

<img width="1120" height="472" alt="Screenshot 2025-10-07 at 00 33 44" src="https://github.com/user-attachments/assets/851ff231-1e48-4459-8947-4a9a76d59753" />

---

## Conference Presentation and Citation

This work was presented at a major international conference in the field of Operational Research - The 33rd European Conference on Operational Research, DTU Denmark, 2024.

### Citing This Work

If you utilise the methodology or results of this project in your own research or publications, please cite the corresponding conference abstract:

**Conference Details:**

* **Conference:** EURO 2024 (The 33rd European Conference on Operational Research)
* **Location:** Copenhagen, Denmark
* **Title:** Manufacturing Process Optimisation and Predictive Analytics: Leveraging Data to Minimise Giveaway in Cheese Production

**Author-Date (Harvard) Style Citation:**

> Iziomo, G. R. (2024). *Product Weight Optimisation to Reduce Giveaway - Causal Inference Analysis and Combinatorial Analysis Using Advanced Analytics and Machine Learning*. Abstract presented at **EURO 2024: The 33rd European Conference on Operational Research**, Copenhagen, Denmark. July 2024. p. 299

The conference abstract book is publicly available:
[https://www.euro-online.org/media\_site/reports/EURO33\_AB.pdf](https://www.euro-online.org/media_site/reports/EURO33_AB.pdf)

---

## Data and Reports Availability

Due to the **commercially sensitive** nature of the proprietary manufacturing data, the detailed **datasets** (`dataset.csv`), the **metadata**, full **project reports** (`Weight Optimisation Report - Aug 2023.pdf, Mini Report - Dec 2023,`, etc.) and slide decks are **confidential** and cannot be made public in this repository.

* **Publicly Available Material:** The project methodology and high-level findings are accessible via the **EURO 2024 conference abstract** and the **presentation slide deck**.
* **Access Request:** To inquire about accessing the non-confidential version of the project report or presentation slides for academic purposes, please contact the lead author **Giwa Reagan Iziomo**.
```
