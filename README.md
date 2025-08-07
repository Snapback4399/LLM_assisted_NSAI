# Neuro-Symbolic AI for Mineral Deposit Classification

This repository contains the code used in the paper **"Enhancing Neuro-Symbolic AI for Mineral Prediction via LLM-Guided Knowledge Integration"**.  
It demonstrates how to integrate domain-specific symbolic knowledge, extracted from geological literature using Large Language Models (LLMs), into machine learning workflows to improve interpretability and predictive performance.

---

## 📂 Contents

### 1. `LLM_Knowledge_match.ipynb`
- Extracts domain knowledge from ore deposit textbooks using LLMs.
- Matches geochemical dataset labels with the extracted knowledge.
- Generates symbolic rules encoded as binary features.

### 2. `LLM_Nsai.ipynb`
- Implements the Neuro-Symbolic AI (NSAI) model.
- Combines raw geochemical features with symbolic knowledge-based features.
- Trains and evaluates baseline ML and NSAI models.
- Uses SHAP and SHAP interaction plots for interpretability.

---

## 🛠 Requirements

Install the dependencies before running the notebooks:

```bash
pip install -r requirements.txt
Key dependencies:

Python 3.9+

Jupyter Notebook

pandas, numpy, scikit-learn

shap

openai (for LLM-based knowledge extraction)

Usage
Knowledge Matching

Open and run LLM_Knowledge_match.ipynb.

Provide access to your geological text data.

The notebook outputs matched features and symbolic rule encodings.

Neuro-Symbolic AI Modeling

Open and run LLM_Nsai.ipynb.

Load your geochemical dataset and symbolic features.

Train baseline ML and NSAI models.

Visualize model interpretability using SHAP.

Outputs
Matched Knowledge Files: Mappings between dataset labels and textbook-derived knowledge.

Model Performance Metrics: Accuracy, precision, recall, F1-score.

SHAP Interaction Plots: Feature interaction importance for baseline and NSAI models.

Citation
If you use this code, please cite:

Chen, W., Leveraging Neuro-Symbolic AI for Enhanced Mineral Prediction in Diverse Copper Deposits. [Conference/Journal], 2025.

License
This repository is licensed under the MIT License. See the LICENSE file for details.
