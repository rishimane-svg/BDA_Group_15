# BDA_Group_15 

Group Members : 

16014223111 - Swara Sawant

16014224802 - Shlok Baraskar 

16014224811 - Rishi Mane

BDA_GROUP_15_IA2 and LabCA 1

# Big Data Analytics for Scholarly Research Intelligence (Topic 20)

This repository contains our IA/CA project for Big Data Analytics (Third-Year AI&DS).
We implement a distributed PySpark pipeline that performs large-scale scholarly literature analysis
and generates SCI-style reporting artifacts for LaTeX integration.

## Project Theme
**Topic 20:** Technical Frameworks for High-Impact Research: Methodologies for Scholarly Writing in Advanced Analytics  
**Case Study:** Creating a technical report draft that synthesizes lab results into a formal SCI-standard research article.

---

## What this project does (pipeline)
- Distributed ingestion of arXiv scholarly metadata
- NLP preprocessing (cleaning, tokenization, stop-word removal)
- Unsupervised clustering (K-Means) for research theme discovery / gap analysis
- Cluster interpretation via top keywords per cluster
- PCA (2D) visualization for cluster separability evidence
- Trend forecasting (publication counts by year and cluster)
- Auxiliary supervised evaluation (Logistic Regression) to report Accuracy/Precision/Recall/F1
- Social impact mapping (keyword-based tagging into Healthcare/Climate/Wildlife)
- Blockchain-style provenance (SHA-256 signatures for record integrity)
- Export of tables/figures/logs and SCI-ready paragraphs for LaTeX chapter writing

All generated artifacts are stored in `outputs/`.

---

## Repository Structure
- `notebooks/` — final documented Colab notebook (`.ipynb`)
- `outputs/figures/` — publication-ready figures (300 DPI)
- `outputs/tables/` — CSV tables for LaTeX Results section
- `outputs/logs/` — reproducibility logs (`run_log.json`)
- `paper/` — LaTeX template + chapter draft + bibliography

---

## Key Outputs (from our run)
- Figures:
  - `outputs/figures/pca_gap_analysis.png`
  - `outputs/figures/trend_forecast.png`
- Tables:
  - `outputs/tables/supervised_metrics.csv`
  - `outputs/tables/runtime_seconds.csv`
  - `outputs/tables/cluster_distribution.csv`
  - `outputs/tables/social_impact_summary.csv`
- Logs:
  - `outputs/logs/run_log.json`

---

## How to Run
```bash
pip install -r requirements.txt
jupyter notebook notebooks/BDA_CODE_2_Topic20_A_GRADE_final.ipynb
