# Credora — AI-Powered Loan & Fraud Risk Intelligence System

## Overview
Built an end-to-end ML system to automate loan approval 
and fraud detection for banking institutions — replacing 
manual review processes that caused high operational costs 
and missed fraud cases.

Most existing tools handle loan approval OR fraud detection 
separately. Credora integrates both into a single 
intelligent pipeline.

## Results
- 34% improvement in fraud catch rate over baseline
- False positive rate reduced to under 6%
- Processed and analyzed 50,000+ loan application records
- Unified 2D risk scoring framework combining default 
  probability and fraud anomaly scores

## Technical Approach

### Loan Approval Pipeline
- Started with Logistic Regression as baseline
- Upgraded to XGBoost ensemble after benchmarking
- Feature engineering on applicant financial data
- Evaluated using Precision, Recall and F1-Score

### Fraud Detection Pipeline
- Used unsupervised methods due to sparse/unreliable 
  fraud labels
- Isolation Forest for statistical anomaly detection
- Autoencoder neural network for reconstruction 
  error based detection
- Combined both scores into unified fraud risk score

### Risk Scoring Framework
- 2D scoring combining loan default probability 
  with fraud anomaly score
- Single interpretable score for bank employees
- Reduces manual review burden significantly

## Why Unsupervised for Fraud?
Fraud labels in banking are often incomplete — 
fraud goes undetected or is discovered months later. 
Supervised models trained on incomplete labels perform 
poorly. Isolation Forest and Autoencoders learn what 
"normal" looks like and flag deviations — no labels needed.

## Tech Stack
Python, Pandas, NumPy, Scikit-learn, XGBoost, 
TensorFlow, Keras, Matplotlib, Seaborn
