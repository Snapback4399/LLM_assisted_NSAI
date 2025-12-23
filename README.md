# Neuro-Symbolic AI for Mineral Deposit Classification

This repository contains the code used in the paper **"Enhancing Neuro-Symbolic AI for Mineral Prediction via LLM-Guided Knowledge Integration"**.  
It demonstrates how to integrate domain-specific symbolic knowledge, extracted from geological literature using Large Language Models (LLMs), into machine learning workflows to improve interpretability and predictive performance.

---

##  Contents

### 1. `LLM_Knowledge_match.ipynb`
- Extracts domain knowledge from ore deposit textbooks using LLMs.
- Matches geochemical dataset labels with the extracted knowledge.
- Generates symbolic rules encoded as binary features.

### 2. `LLM_Nsai.ipynb`
- Implements the Neuro-Symbolic AI (NSAI) model.
- Combines raw geochemical features with symbolic knowledge-based features.
- Trains and evaluates baseline ML and NSAI models.
- Uses SHAP and SHAP interaction plots for interpretability.




## Requirements

Install the dependencies before running the notebooks:

Key dependencies:

Python 3.9+

Jupyter Notebook

pandas, numpy, scikit-learn

shap

openai (for LLM-based knowledge extraction)
