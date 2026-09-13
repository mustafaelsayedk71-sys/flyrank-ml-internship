# FlyRank AI Capstone — Content Action & Valuation Engine

**Author:** Mustafa Elsayed  
**Track:** General AI Fluency / Machine Learning (Week 8 Final Checkpoint)  
**Live Demo Video:** https://youtu.be/YOUR_DEMO_VIDEO_LINK  
**Live Deployed Site:** https://mustafaelsayedk71-sys.github.io/portfolio/  

---

## Overview & Architecture
This repository implements an automated machine learning evaluation and site-hardening workflow designed to analyze content decay across search impression logs. It replaces intuition-based content refreshes with ranked, leakage-free heuristic and regression models.

### System Architecture Sketch
`Raw Data (CSV)` ➡️ `GroupKFold Validation` ➡️ `Random Forest Scoring Engine` ➡️ `Action Archetype Triage` ➡️ `Static Site Dashboard Deployment`

---

## Setup & Local Execution Guide
Follow these exact steps to replicate the execution environment locally:

```bash
# 1. Clone the repository
git clone [https://github.com/mustafaelsayedk71/flyrank-ml-internship.git](https://github.com/mustafaelsayedk71/flyrank-ml-internship.git)
cd flyrank-ml-internship

# 2. Install required dependencies
pip install pandas numpy scikit-learn matplotlib

# 3. Execute the capstone notebook
jupyter notebook work/notebooks/capstone.ipynb
Metric / Model Split,Baseline Heuristic Rule,Random Forest Model (GroupKFold)
Mean Absolute Error (MAE),1450.20,920.40
Data Leakage Mitigation,None (Random Split),Protected (Domain-Grouped Split)
Limitations List
Directional Predictions: Model valuation outputs act as decision-support signals rather than absolute traffic guarantees.

API Rate Limits: Form submission endpoints on the portfolio showcase use free-tier third-party routing caps.

AI Transparency & AI Partnership Statement
This project was built in collaboration with AI assistance (Claude / ChatGPT / Gemini). AI was used for architectural brainstorming, boilerplate setup, and initial refactoring. All core validation logic (GroupKFold leakage prevention), feature thresholds, and code verification were manually audited, evaluated, and tested by me.
