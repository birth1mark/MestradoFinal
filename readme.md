# Trust-DT: A Synergistic Framework for Trustworthy Healthcare Digital Twins

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.20083912.svg)](https://doi.org/10.5281/zenodo.20083912)

This repository contains the implementation of the **Trust-DT** framework, developed as part of my Master's research in Web Technologies and Systems Engineering at ISLA Gaia.

Trust-DT addresses the "trust gap" in clinical Digital Twin adoption by treating **Explainability** and **Uncertainty Quantification** as core engineering requirements rather than afterthoughts.

## 🔬 Scientific Context
Healthcare Digital Twins (DTs) offer immense potential for personalized medicine. However, clinical adoption is often throttled by overconfident "black-box" AI models. Trust-DT provides a modular audit layer to ensure that clinical predictions are not just accurate, but statistically reliable.

## 📖 Publications and Academic Impact
This project is associated with the peer-reviewed article: 
*"Trust-DT: A Synergistic Framework for Trustworthy Healthcare Digital Twins via Explainable AI and Statistical Calibration"*.

* **Read on Academia.edu:** [https://www.academia.edu/167681833/Trust_DT_A_Synergistic_Framework_for_Trustworthy_Healthcare_Digital_Twins_via_Explainable_AI_and_Statistical_Calibration](https://www.academia.edu/167681833/Trust_DT_A_Synergistic_Framework_for_Trustworthy_Healthcare_Digital_Twins_via_Explainable_AI_and_Statistical_Calibration)
* **Access Official Repository (Zenodo):** [https://doi.org/10.5281/zenodo.20083912](https://doi.org/10.5281/zenodo.20083912)

## 🛠 Methodology
The framework implements a dual-layered audit system:
1. **Explainability (XAI):** Integration of SHAP and LIME to interpret feature importance in clinical decisions.
2. **Uncertainty Quantification (UQ):** Utilization of **Conformal Prediction** (via MAPIE) to provide rigorous confidence sets, preventing overconfident clinical errors.

## 📊 Performance Analysis
Key findings from the implementation:
* **Base Model (XGBoost/RF):** Achieved 87.19% accuracy.
* **The Calibration Crisis:** Revealed that empirical coverage collapsed to ~24% under a 90% target confidence level without proper calibration.
* **Trust-DT Impact:** Successfully bridges the coverage gap, ensuring model outputs align with clinical safety standards.

## 🚀 Getting Started

### Prerequisites
* Python 3.10+
* `scikit-learn`, `mapie`, `shap`, `xgboost`, `pandas`, `numpy`

### Installation
```bash
git clone [https://github.com/yourusername/Trust-DT.git](https://github.com/yourusername/Trust-DT.git)
cd Trust-DT
pip install -r requirements.txt
