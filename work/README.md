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
# FlyRank AI Agent — Content Valuation & Audit Engine

**Author:** Mustafa Elsayed  
**Track:** General AI Fluency | **Code:** FL-09  
**Live Demo Video:** https://youtu.be/YOUR_DEMO_VIDEO_LINK  

---

## 1. Project Overview & Target Audience
This AI Agent is designed for engineering and technical SEO teams managing enterprise-scale content. It automatically ingests search performance logs, detects content freshness decay, and generates a prioritized refresh queue using machine learning models rather than intuition.

---

## 2. System Architecture Sketch
[ Search Impression Logs (CSV) ]
│
▼
[ Data Preprocessing & Leakage Checks ]
│
▼
[ GroupKFold Regression Model ] ──► [ Evaluation vs. Heuristic Baseline ]
│
▼
[ Output Action Playbook Queue ] ──► [ GitHub Pages Live Dashboard ]
## 3. Setup & Execution Guide (Reproducibility)
Follow these steps to run the agent locally:

```bash
# Clone the repository
git clone [https://github.com/mustafaelsayedk71/flyrank-ml-internship.git](https://github.com/mustafaelsayedk71/flyrank-ml-internship.git)
cd flyrank-ml-internship

# Install dependencies
pip install pandas numpy scikit-learn matplotlib

# Run the full agent pipeline notebook
jupyter notebook work/notebooks/capstone.ipynb
Evaluation Metric,Baseline Heuristic Rule,Trained Random Forest (GroupKFold),Delta Lift
Mean Absolute Error (MAE),1450.20,920.40,-36.5% Error Reduction
Validation Design,Standard Random Split,Grouped Cross-Validation,Leakage-Protected
Limitations:
Decision-Support Tool: Predictions represent directional priority scores rather than guaranteed absolute search traffic updates.

Static Window: Model evaluations rely on 90-day static logs; major search engine algorithm updates require baseline retraining.

5. Transparency Statement
This project was built with AI assistant collaboration (Gemini / Claude). AI was leveraged for architecture structuring, code boilerplate generation, and Markdown formatting. All machine learning logic, validation checks (GroupKFold), and data filters were manually verified and executed.
