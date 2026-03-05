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

### Boosted Decision Trees (BDT)
Implemented using scikit-learn / TMVA-style workflows.

### XGBoost
Gradient boosted decision trees optimized for performance and scalability.

The training pipeline includes:

- Feature selection
- Dataset splitting (training / validation)
- Cross-validation
- Hyperparameter tuning

---

## Evaluation Metrics

Model performance is evaluated using:

- ROC curves
- Area Under Curve (AUC)
- Classification accuracy
- Signal significance estimates

Example output includes:

- ROC comparison between BDT and XGBoost
- Feature importance ranking
- Confusion matrices


