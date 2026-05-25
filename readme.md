Trust-DT: A Synergistic Framework for Trustworthy Healthcare Digital Twins
This repository contains the implementation of the Trust-DT framework, developed as part of my Master's research in Web Technologies and Systems Engineering at ISLA Gaia.

Trust-DT addresses the "trust gap" in clinical Digital Twin adoption by treating Explainability and Uncertainty Quantification as core engineering requirements rather than afterthoughts.

🔬 Scientific Context
Healthcare Digital Twins (DTs) offer immense potential for personalized medicine. However, clinical adoption is often throttled by overconfident "black-box" AI models. Trust-DT provides a modular audit layer to ensure that predictions are not just accurate, but statistically reliable.

🛠 Methodology
The framework implements a dual-layered audit system:

Explainability (XAI): Integration of SHAP and LIME to interpret feature importance in clinical decisions.

Uncertainty Quantification (UQ): Utilization of Conformal Prediction (via MAPIE) to provide rigorous confidence sets, preventing overconfident clinical errors.

📊 Performance Analysis
Key findings from the implementation:

Base Model (XGBoost/RF): Achieved 87.19% accuracy.

The Calibration Crisis: Revealed that empirical coverage collapsed to ~24% under a 90% target confidence level without proper calibration.

Trust-DT Impact: Successfully bridges the coverage gap, ensuring model outputs align with clinical safety standards.

🚀 Getting Started
Prerequisites
Python 3.10+

scikit-learn, mapie, shap, xgboost, pandas, numpy

Installation
Bash
git clone https://github.com/yourusername/Trust-DT.git
cd Trust-DT
pip install -r requirements.txt
Execution
To replicate the calibration analysis:

Bash
python main_calibration_analysis.py --model xgboost --alpha 0.1
📜 How to Cite
If you use this framework in your research, please cite the original publication:

DOI: 10.5281/zenodo.20083912

Citation: Ribeiro, P. (2026). Trust-DT: A Synergistic Framework for Trustworthy Healthcare Digital Twins via Explainable AI and Statistical Calibration.

⚖️ License
This project is licensed under the MIT License. Feel free to use, modify, and contribute to this research.
