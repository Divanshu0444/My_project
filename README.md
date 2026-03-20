# Machine Learning Classification of Higgs Jets in ttH Events

This project applies machine learning techniques to classify jets originating from Higgs boson decays in the \( t\bar{t}H \) production channel at the Large Hadron Collider (LHC).

The goal is to distinguish Higgs decay products from background jets using kinematic features and multivariate classifiers such as Boosted Decision Trees (BDT) and XGBoost.

This work was developed as part of a High Energy Physics analysis project at IIT Madras.

---

## Physics Motivation

The \( t\bar{t}H \) process provides a direct probe of the Higgs-top Yukawa coupling, an important parameter in the Standard Model.

Identifying Higgs-origin jets in these events is challenging due to large combinatorial backgrounds from top-quark decays and additional QCD jets.

Machine learning methods can improve the separation between signal and background by exploiting correlations among kinematic variables.

---

## Dataset

The analysis uses simulated event data containing reconstructed jet and particle-level features relevant to the \( t\bar{t}H \) final state.

Typical features include:

- Jet transverse momentum (pT)
- Jet pseudorapidity (η)
- Jet invariant mass
- Angular separation variables (ΔR)
- Event-level kinematic observables

The dataset is prepared as structured arrays and used for supervised binary classification.

---

## Machine Learning Methods

Two multivariate classifiers are implemented:

### XGBoost
Gradient boosted decision trees optimized for performance and scalability.

- Feature selection  
- Train/validation split  
- Cross-validation and hyperparameter tuning  

### Deep Neural Network (DNN)
Fully connected neural network for learning complex non-linear patterns.

- Input normalization  
- Train/validation split  
- Model training and evaluation using ROC and significance metrics  
---

## Evaluation Metrics

Model performance is evaluated using:

- ROC curves
- Area Under Curve (AUC)
- KS test 
- Signal significance estimates


