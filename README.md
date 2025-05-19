# Understanding-Causal-Inference-with-Statistical-and-Machine-Learning-Models
# Causal Inference Analysis: Impact of Specialized Childcare on Cognitive Development 🧠📊

[![Python 3.8+](https://img.shields.io/badge/python-3.8%2B-blue)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.XXXXXXX.svg)](https://doi.org/10.5281/zenodo.XXXXXXX)

*A comprehensive causal inference study using advanced statistical and machine learning techniques to evaluate early childhood interventions.*

## 🌟 Highlights

- **Robust Causal Analysis**: Implements 3 distinct methodologies (IPW, DML, CFR) for treatment effect estimation
- **Real-World Impact**: Analyzes IHDP dataset containing 747 premature infants' developmental data
- **Advanced ML Integration**: Combines traditional statistics with Random Forests and Deep Learning
- **Transparent Science**: Full reproducibility with Jupyter notebooks and detailed documentation
- **Visual Analytics**: Interactive plots for propensity scores, ROC curves, and treatment effect distributions

## 📚 Table of Contents
- [Key Findings](#-key-findings)
- [Methodologies](#-methodologies)
- [Dataset](#-dataset)
- [Installation](#-installation)
- [Usage](#-usage)
- [Visualizations](#-visualizations)
- [Ethical Considerations](#-ethical-considerations)
- [Future Work](#-future-work)
- [Credits](#-credits)

## 🔍 Key Findings
- **+4.01 Point Cognitive Gain**: Specialized childcare shows significant positive impact (p<0.01)
- **Model Comparison**:
  - Double Machine Learning: 3.80 ATE (95% CI: 3.70-3.90)
  - Counterfactual Regression: 4.09 ATE 
  - Inverse Probability Weighting: 3.06 ATE
- **Critical Covariates**: Maternal education and birth weight identified as key effect modifiers

## 🛠 Methodologies
### Advanced Causal Techniques Implemented
| Method | Key Strength | Implementation Detail |
|--------|--------------|-----------------------|
| **IPW** | Confounder Adjustment | Logistic Regression with Stabilized Weights |
| **DML** | Double Robustness | Random Forest + Residualization |
| **CFR** | Counterfactual Prediction | Deep Neural Network with MMD Regularization |


## 📦 Dataset
**Infant Health and Development Program (IHDP)**
- 747 preterm infants with 25 pre-treatment covariates
- Features: Maternal education, birth weight, household income
- Semi-synthetic outcomes with known ground truth

[![IHDP Dataset Sample](https://via.placeholder.com/800x200.png?text=Dataset+Snapshot)](your-dataset-image-link)

## ⚙ Installation


## 🖥 Usage
1. **Exploratory Analysis**:


2. **Run Full Analysis**:


## 📊 Visualizations
### Key Analytical Graphics
| Visualization | Insight | Technical Detail |
|---------------|---------|------------------|
| ![SMD Plot](https://via.placeholder.com/150x150.png?text=SMD) | Covariate Balance | Standardized Mean Differences |
| ![ROC Curve](https://via.placeholder.com/150x150.png?text=ROC) | Model Performance | AUC = 0.744 |
| ![ATE Comparison](https://via.placeholder.com/150x150.png?text=ATE) | Treatment Effects | Error Bar Visualization |

## 🤝 Ethical Considerations
- **Data Anonymization**: All personal identifiers removed from IHDP dataset
- **Algorithmic Fairness**: Regular bias checks using Aequitas toolkit
- **Reproducibility**: Full Docker environment included

## 🚀 Future Work
- [ ] Implement Causal Forest algorithm
- [ ] Add sensitivity analysis for unobserved confounding
- [ ] Develop interactive Shiny dashboard

## 📜 Credits
**Supervisor**: Prof. Sharmishtha Mitra, Department of Mathematics & Statistics  
**Institutional Support**: Indian Institute of Science Education and Research (IISER)  

*"The true logic of this world is in the calculus of probabilities."* - James Clerk Maxwell

