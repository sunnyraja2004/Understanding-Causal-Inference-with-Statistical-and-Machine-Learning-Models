Understanding Causal Inference with Statistical and Machine Learning Models
MS Project 2: Advanced Causal Analysis and Robustness Extensions 🧠📈

Python 3.8+ | License: MIT | DOI: (to be assigned)

This repository presents MS Project 2, a methodological continuation of MS Project 1, which extends the causal inference analysis of early childhood interventions with robustness checks, heterogeneity analysis, and advanced causal machine learning models.

The study continues to evaluate the causal impact of specialized childcare on cognitive development using the IHDP dataset, with a focus on validity, interpretability, and policy relevance.

🌟 Highlights (Project 2 Additions)

Beyond Average Effects
Moves from ATE estimation to treatment effect heterogeneity (HTE) and subgroup analysis

Robustness & Sensitivity Analysis
Explicit assessment of stability under model choice and potential unobserved confounding

Advanced Causal ML
Extension to flexible learners and representation-based causal models

Comparative Framework
Systematic comparison of causal estimators across assumptions and modeling choices

Research Continuity
Fully reproducible extension of MS Project 1 with shared data pipeline and preprocessing

📚 Table of Contents

Project Overview

Relationship to MS Project 1

Key Contributions (Project 2)

Methodologies

Dataset

Installation

Usage

Visualizations

Ethical Considerations

Limitations

Future Work

Credits

🔍 Project Overview

Early childhood interventions are known to influence long-term cognitive outcomes, but causal estimation remains challenging due to confounding and selection bias.

MS Project 2 builds on the baseline causal estimates from MS Project 1 by:

Examining robustness of treatment effects

Investigating heterogeneous treatment effects

Studying estimator behavior under different modeling assumptions

The objective is not only estimation accuracy, but causal credibility.

🔗 Relationship to MS Project 1
Aspect	MS Project 1	MS Project 2
Focus	Average Treatment Effect	Heterogeneity & Robustness
Methods	IPW, DML, CFR	Extended DML, Representation Learning, Sensitivity Checks
Outcome	Point estimates	Stability, subgroup effects, uncertainty
Goal	Causal estimation	Causal understanding

Project 2 does not replace Project 1 — it strengthens and interrogates its conclusions.

🧠 Key Contributions (MS Project 2)

Treatment Effect Heterogeneity
Evidence of variation in cognitive gains across:

Maternal education levels

Birth weight categories

Socio-economic indicators

Estimator Stability
Comparison of causal estimates under:

Different nuisance learners

Alternative propensity specifications

Interpretability
Identification of covariates acting as effect modifiers, not just confounders

Methodological Insight
Highlights where causal ML models agree — and where they diverge

🛠 Methodologies
Causal Techniques Used
Method	Purpose	Key Idea
IPW	Baseline adjustment	Weighted pseudo-population
DML (Extended)	Double robustness	Orthogonalization with ML
CFR	Counterfactual learning	Balanced representations
Subgroup Analysis	HTE estimation	Conditional effects
Sensitivity Analysis	Robustness	Assess hidden bias impact

Machine learning components include Random Forests and Neural Networks, used strictly as nuisance models, not causal objects.

📦 Dataset

Infant Health and Development Program (IHDP)

747 preterm infants

25 pre-treatment covariates

Semi-synthetic outcomes with known structure

Widely used benchmark for causal inference research

The same dataset and preprocessing pipeline as MS Project 1 are retained for comparability.

⚙ Installation
git clone https://github.com/your-username/Understanding-Causal-Inference.git
cd Understanding-Causal-Inference
pip install -r requirements.txt


(Optional) A Docker environment is provided for full reproducibility.

🖥 Usage
Exploratory Data Analysis
notebooks/01_exploratory_analysis.ipynb

Baseline Causal Models (Project 1)
notebooks/02_ipw_dml_cfr.ipynb

Heterogeneity & Robustness (Project 2)
notebooks/03_heterogeneity_analysis.ipynb
notebooks/04_sensitivity_checks.ipynb

📊 Visualizations
Visualization	Purpose
Covariate Balance (SMD)	Overlap & adjustment quality
Propensity Score Distributions: Positivity Assessment
ATE & HTE Plots	Effect comparison
Subgroup Effect Charts	Interpretability
Sensitivity Curves	Robustness diagnostics

All figures are reproducible from notebooks.

🤝 Ethical Considerations

Data Privacy: IHDP data is fully anonymized

Bias Awareness: Explicit checks for model-induced disparities

Interpretation Caution: Results framed as causal estimates, not guarantees

Transparency: All assumptions are clearly stated and tested where possible

⚠ Limitations

No experimental randomization

Sensitivity analysis cannot entirely rule out unobserved confounding.

Results specific to the IHDP population

Neural models improve flexibility, not causal certainty.

These limitations are explicitly discussed in the report.

🚀 Future Work

Causal Forests and Bayesian Causal Models

Formal bounds for unobserved confounding

Long-term outcome extensions

Policy simulation under heterogeneous effects

📜 Credits

Student: Sunny
Supervisor: Prof. Sharmishtha Mitra
Department: Mathematics & Statistics
Institution: Indian Institute of Science Education and Research (IISER)

“The true logic of this world is in the calculus of probabilities.”
— James Clerk Maxwell

