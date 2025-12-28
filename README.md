# Understanding Causal Inference with Statistical and Machine Learning Models
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

