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

> **Note:**  
> In this implementation, symbolic knowledge representations are constructed with access to deposit-model information prior to model training.  
> This setup is intended to evaluate the *upper-bound contribution* of domain knowledge under idealized conditions, rather than to represent a fully label-independent deployment pipeline.
> For readers interested in a label-independent implementation under realistic prediction settings, an alternative supplementary pipeline is available at: https://github.com/Snapback4399/LLM_assisted_NSAI_sup/
> Thanks to Dr. Jeffrey M. Dick of Central South University, China for spotting this as a data leakage issue and contacting us immediately two weeks after the original article was published online. 
---


## Requirements

Install the dependencies before running the notebooks:

Key dependencies:

Python 3.9+

Jupyter Notebook

pandas, numpy, scikit-learn

shap

openai (for LLM-based knowledge extraction)
