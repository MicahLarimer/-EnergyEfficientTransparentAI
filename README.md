# EnergyEfficientTransparentAI

**A work-in-progress project to revolutionize AI with energy-efficient and transparent models, targeting healthcare applications.**

## Overview
This project develops energy-efficient and interpretable AI models, starting with a neural network classifier for the Iris dataset. It’s a stepping stone toward larger goals: building sustainable, transparent AI systems for real-world applications like healthcare diagnostics. By integrating tools like CodeCarbon for emissions tracking and SHAP for interpretability, the project aligns with the vision of revolutionizing AI to be greener and more trustworthy.

## Current Features
- **Iris Classifier** (`notebooks/fastai_lesson2_iris.ipynb`):
  - Built a tabular neural network using `fastai` and `pandas` to classify Iris flowers (setosa, versicolor, virginica) with **96.67% accuracy**.
  - Optimized with `layers=[50,25]`, `bs=10`, and `lr_max=1e-2`, analyzing misclassifications (e.g., versicolor as virginica).
  - Integrated **CodeCarbon** for eco-friendly AI, achieving **0.000027 kg CO2 emissions**.
  - Added **SHAP** for interpretability, visualizing feature contributions (e.g., petal length’s impact) via summary and force plots (`plots/shap_summary.png`, `plots/shap_force_misclassified.png`).
- **Work in Progress**:
  - Exploring **MIMIC-III** dataset for healthcare AI (e.g., predicting hospital readmissions).
  - Planning **EfficientNet-B0 pruning** to reduce model size and energy use for image-based applications.
  - Learning from fast.ai course (Lessons 2–10) to enhance tabular and vision model skills.

## Vision
This project is part of a broader mission to revolutionize AI by:
- **Reducing Energy Use**: Minimizing computational footprints (e.g., via model pruning and CodeCarbon tracking) to make AI sustainable.
- **Enhancing Transparency**: Using tools like SHAP to explain model decisions, building trust in critical domains like healthcare.
- **Scaling to Healthcare**: Applying efficient, interpretable models to datasets like MIMIC-III for real-world impact (e.g., diagnostic predictions).

## Getting Started
### Prerequisites
- Python 3.11
- Libraries: `fastai`, `pandas`, `scikit-learn==1.5.0`, `codecarbon==3.0.2`, `shap`, `matplotlib`
- Install via:
  ```bash
  conda create -n fastai_env python=3.11
  conda activate fastai_env
  pip install fastai pandas scikit-learn==1.5.0 codecarbon==3.0.2 shap matplotlib