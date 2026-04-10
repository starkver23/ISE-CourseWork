# Intelligent Bug Report Classification Tool

**Author:** Aryan Verma  
**Project Type:** MSc Advanced Computer Science - Tool Building Coursework  
**University:** University of Birmingham

---

## 📝 Project Overview

This repository contains an intelligent software engineering tool designed to automate the classification of user-submitted bug reports for the **PyTorch** project. The tool addresses the challenge of manual triaging by distinguishing between "Bugs" and "Other" reports using advanced Natural Language Processing (NLP) techniques.

## 🚀 Key Results

The proposed tool significantly outperforms the course baseline (Gaussian Naive Bayes) across all critical metrics:

- **Accuracy:** 88.08% (Baseline: 62.58%)
- **Macro F1-Score:** 0.7280 (Baseline: 0.5551)
- **Statistical Significance:** Wilcoxon p-value = 0.00195 ($p < 0.05$)

## 🧠 Intelligence Features

- **Advanced Preprocessing:** Implementation of **WordNet Lemmatization** to reduce vocabulary noise and improve pattern recognition.
- **Balanced Learning:** Utilized cost-sensitive learning (`class_weight='balanced'`) to mitigate class imbalance.
- **Optimized Algorithms:** Comparison of multiple models, with **Logistic Regression** identified as the most effective for sparse TF-IDF feature spaces.

---

## 📂 Repository Structure

- `ToolBuilding.py`: Final multi-model experimental script.
- `requirements.pdf`: Detailed environment and dependency list.
- `manual.pdf`: Instructions for setup and execution.
- `replication.pdf`: Parameters required to reproduce report findings.
- `results/`: Folder containing performance graphs and raw metrics.

## 🛠️ Quick Start

1. Ensure the `pytorch.csv` dataset is located in a `datasets/` folder.
2. Install dependencies listed in `requirements.pdf`.
3. Run the analysis:
   ```bash
   python ToolBuilding.py
   ```
