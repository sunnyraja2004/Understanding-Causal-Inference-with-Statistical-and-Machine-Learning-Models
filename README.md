# Understanding Causal Inference with Statistical and Machine Learning Models
# 🧠 MS Project 3: Causal Inference under Endogeneity using Instrumental Variables and Double Machine Learning

## Overview

MS Project 3 extends the causal inference framework developed in the previous projects to settings with **endogenous treatment assignment**, where treatment participation depends on unobserved factors that also affect outcomes.

The project studies the causal effect of **401(k) retirement plan participation** on household financial wealth using a combination of **classical econometric methods** and **modern machine learning approaches**. Specifically, it integrates **Instrumental Variables (IV)**, **Two-Stage Least Squares (2SLS)**, and **Double Machine Learning for Instrumental Variables (DMLIV)** to estimate both average and heterogeneous causal effects.

---

## 🔗 Relationship to Previous Projects

| Aspect         | MS Project 1              | MS Project 2                            | MS Project 3                            |
| -------------- | ------------------------- | --------------------------------------- | --------------------------------------- |
| Focus          | Average Treatment Effects | Heterogeneity & Robustness              | Endogeneity & Heterogeneous IV Effects  |
| Identification | Unconfoundedness          | Unconfoundedness                        | Instrumental Variables                  |
| Methods        | IPW, DML                  | Extended DML, CFR, Sensitivity Analysis | IV, 2SLS, DMLIV                         |
| Outcome        | Average Effects           | Subgroup Effects                        | Heterogeneous LATE                      |
| Goal           | Causal Estimation         | Causal Understanding                    | Causal Identification under Endogeneity |

Project 3 builds upon the treatment-effect estimation framework developed in Projects 1 and 2 while addressing realistic settings where treatment assignment is endogenous.

---

## 🌟 Highlights (Project 3 Additions)

* Instrumental Variable identification for endogenous treatment assignment
* Two-Stage Least Squares (2SLS) estimation
* Wu–Hausman and Sargan diagnostic testing
* Double Machine Learning for Instrumental Variables (DMLIV)
* Heterogeneous Local Average Treatment Effects (LATE)
* Bootstrap inference and confidence intervals
* Repeated cross-fitting for estimator stability
* Weak-instrument robust inference
* Policy targeting analysis
* Distributional treatment-effect analysis

---

## 🎯 Objective

To estimate the causal effect of **401(k) participation** on household financial wealth when participation decisions are endogenous and influenced by unobserved characteristics such as financial literacy, risk preferences, and saving behavior.

---

## 📊 Dataset

### 401(k) Pension Dataset

* 9,915 household observations
* Cross-sectional observational data
* Endogenous treatment assignment
* Widely used benchmark in econometrics

### Key Variables

**Outcome**

* Net Financial Assets (`net_tfa`)

**Treatment**

* 401(k) Participation (`p401`)

**Instruments**

* 401(k) Eligibility (`e401`)
* Eligibility × Dual-Earner Status (`e401 × twoearn`)

**Controls**

* Age
* Income
* Education
* Family Size
* Marital Status
* IRA Participation
* Home Ownership
* Defined Benefit Pension Status

---

## 🛠 Methodologies

### Classical Econometric Methods

| Method          | Purpose                |
| --------------- | ---------------------- |
| OLS             | Baseline estimation    |
| IV              | Endogeneity correction |
| 2SLS            | Causal estimation      |
| Wu–Hausman Test | Endogeneity detection  |
| Sargan Test     | Instrument validity    |

### Modern Causal Machine Learning

| Method                  | Purpose                    |
| ----------------------- | -------------------------- |
| DMLIV                   | Heterogeneous IV effects   |
| Orthogonalization       | Bias reduction             |
| Cross-Fitting           | Robust estimation          |
| Bootstrap Inference     | Uncertainty quantification |
| Policy Targeting Curves | Decision support           |

---

## 🔬 Key Results

### Classical IV Results

| Estimator | Effect (USD) |
| --------- | ------------ |
| OLS       | $14,620      |
| 2SLS      | $8,450       |

The gap between OLS and IV estimates highlights substantial upward bias caused by endogenous participation decisions.

### DMLIV Results

* Average Heterogeneous Effect ≈ $11,390
* Strong treatment-effect heterogeneity across households
* Significant variation across income groups and age cohorts

### Income Heterogeneity

Average gains increase monotonically across income levels:

| Income Group   | Mean Effect |
| -------------- | ----------- |
| Lowest Decile  | $4,460      |
| Highest Decile | $26,530     |

### Age Heterogeneity

Average gains increase with age:

| Age Group         | Mean Effect |
| ----------------- | ----------- |
| Youngest Quartile | $4,960      |
| Oldest Quartile   | $19,810     |

---

## 📈 Policy Insights

* High-income households experience substantially larger gains from 401(k) participation.
* Treatment effects increase throughout the life cycle.
* Targeting individuals with the highest predicted gains can generate more than double the aggregate benefits of untargeted policies.
* Retirement savings incentives exhibit strong heterogeneity across demographic groups.

---

## 🔍 Research Contributions

* Endogeneity-aware causal inference
* Instrumental variable identification
* Heterogeneous Local Average Treatment Effects (LATE)
* Econometric and machine learning integration
* Policy-targeting frameworks
* Robust causal inference under observational settings

---

## 🚀 Project Sequence

### MS Project 1

Average Treatment Effect Estimation under Unconfoundedness

### MS Project 2

Treatment Effect Heterogeneity, Robustness Analysis, and Advanced Causal Machine Learning

### MS Project 3

Endogeneity, Instrumental Variables, DMLIV, and Policy-Relevant Heterogeneous Causal Effects

Together, the three projects provide a complete progression from classical treatment-effect estimation to modern machine learning–based causal inference under realistic observational settings.

## MS Project 2: Advanced Causal Analysis and Robustness Extensions 🧠📈

**Python 3.8+ | License: MIT | DOI: (to be assigned)**

This repository presents **MS Project 2**, a methodological continuation of **MS Project 1**, which extends the causal inference analysis of early childhood interventions with:

- **Robustness checks**
- **Heterogeneity analysis**
- **Advanced causal machine learning models**

The study continues to evaluate the causal impact of specialized childcare on **cognitive development** using the **IHDP dataset**, focusing on **validity, interpretability, and policy relevance**.

---

## 🌟 Highlights (Project 2 Additions)

- **Beyond Average Effects**: Moves from **ATE estimation** to **treatment effect heterogeneity (HTE)** and **subgroup analysis**  
- **Robustness & Sensitivity Analysis**: Explicit assessment of stability under **model choice** and **potential unobserved confounding**  
- **Advanced Causal ML**: Extension to flexible learners and **representation-based causal models**  
- **Comparative Framework**: Systematic comparison of **causal estimators** across assumptions and modeling choices  
- **Research Continuity**: Fully reproducible extension of MS Project 1 with shared **data pipeline** and **preprocessing**

---

## 📚 Table of Contents

1. [Project Overview](#project-overview)  
2. [Relationship to MS Project 1](#relationship-to-ms-project-1)  
3. [Key Contributions (Project 2)](#key-contributions-ms-project-2)  
4. [Methodologies](#methodologies)  
5. [Dataset](#dataset)  
6. [Installation](#installation)  
7. [Usage](#usage)  
8. [Visualizations](#visualizations)  
9. [Ethical Considerations](#ethical-considerations)  
10. [Limitations](#limitations)  
11. [Future Work](#future-work)  
12. [Credits](#credits)

---

## 🔍 Project Overview

Early childhood interventions are known to influence long-term **cognitive outcomes**, but **causal estimation** remains challenging due to **confounding** and **selection bias**.  

**MS Project 2** builds on the baseline causal estimates from **MS Project 1** by:

- Examining **robustness** of treatment effects  
- Investigating **heterogeneous treatment effects**  
- Studying **estimator behavior** under different modeling assumptions  

**Objective:** Not only estimation accuracy, but **causal credibility**.

---

## 🔗 Relationship to MS Project 1

| Aspect | MS Project 1 | MS Project 2 |
|--------|--------------|--------------|
| **Focus** | Average Treatment Effect | Heterogeneity & Robustness |
| **Methods** | IPW, DML, CFR | Extended DML, Representation Learning, Sensitivity Checks |
| **Outcome** | Point estimates | Stability, subgroup effects, uncertainty |
| **Goal** | Causal estimation | Causal understanding |

> Project 2 does not replace Project 1 — it strengthens and interrogates its conclusions.

---

## 🧠 Key Contributions (MS Project 2)

- **Treatment Effect Heterogeneity**  
  Variation in cognitive gains across:  
  - **Maternal education levels**  
  - **Birth weight categories**  
  - **Socio-economic indicators**  

- **Estimator Stability**  
  Comparison of causal estimates under:  
  - Different **nuisance learners**  
  - Alternative **propensity specifications**  

- **Interpretability**  
  Identification of covariates acting as **effect modifiers**, not just **confounders**  

- **Methodological Insight**  
  Highlights where **causal ML models** agree — and where they diverge

---

## 🛠 Methodologies

### Causal Techniques Used

| Method | Purpose | Key Idea |
|--------|--------|---------|
| **IPW** | Baseline adjustment | Weighted pseudo-population |
| **DML (Extended)** | Double robustness | Orthogonalization with ML |
| **CFR** | Counterfactual learning | Balanced representations |
| **Subgroup Analysis** | HTE estimation | Conditional effects |
| **Sensitivity Analysis** | Robustness | Assess hidden bias impact |

> Machine learning components include **Random Forests** and **Neural Networks**, used strictly as **nuisance models**, not causal objects.

---

## 📦 Dataset

**Infant Health and Development Program (IHDP)**  

- 747 preterm infants  
- 25 pre-treatment covariates  
- Semi-synthetic outcomes with known structure  
- Widely used benchmark for **causal inference research**  

> The same dataset and preprocessing pipeline as **MS Project 1** are retained for comparability.

---

## ⚙ Installation

```bash
git clone https://github.com/your-username/Understanding-Causal-Inference.git
cd Understanding-Causal-Inference
pip install -r requirements.txt

