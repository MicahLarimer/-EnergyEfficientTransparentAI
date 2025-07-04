# EnergyEfficientTransparentAI

**A work-in-progress project to revolutionize AI with energy-efficient and transparent models, targeting healthcare applications.**

## Overview
This project develops energy-efficient and interpretable AI models, starting with a neural network classifier for the Iris dataset. It’s a foundation for building sustainable, transparent AI systems for applications like healthcare diagnostics. Using tools like CodeCarbon for emissions tracking and SHAP for interpretability, it aims to revolutionize AI by making it greener and more trustworthy.

## Current Features
- **Iris Classifier** (`notebooks/fastai_lesson2_iris.ipynb`):
  - Built a tabular neural network using `fastai` and `pandas` to classify Iris flowers (setosa, versicolor, virginica) with an expected **96.67% accuracy**.
  - Optimized with `layers=[50,25]`, `bs=10`, and `lr_max=1e-2`, with misclassification analysis fixed to handle unique indices correctly (current output shows repeated indices, under review).
  - Integrated **CodeCarbon** for eco-friendly AI, achieving **0.000027–0.000035 kg CO2 emissions** on an AMD Ryzen 3 3250U with 5.922 GB RAM.
  - Added **SHAP** with a custom prediction function, generating a summary plot (`plots/shap_summary.png`) and an interactive force plot (`plots/shap_force_misclassified.html`) for multi-class outputs, revealing key features like [insert top feature, e.g., petal_length] as major contributors (see screenshots at [https://github.com/MicahLarimer/-EnergyEfficientTransparentAI/blob/ca849936316a9aedf54ddddf255d2081bca3b874/Screenshot%202025-07-03%20174220.png](https://github.com/MicahLarimer/-EnergyEfficientTransparentAI/blob/ca849936316a9aedf54ddddf255d2081bca3b874/Screenshot%202025-07-03%20174220.png) and [https://github.com/MicahLarimer/-EnergyEfficientTransparentAI/blob/ca849936316a9aedf54ddddf255d2081bca3b874/Screenshot%202025-07-03%20181403.png](https://github.com/MicahLarimer/-EnergyEfficientTransparentAI/blob/ca849936316a9aedf54ddddf255d2081bca3b874/Screenshot%202025-07-03%20181403.png) for details, pending full SHAP completion).
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
- Libraries: `fastai`, `pandas`, `scikit-learn==1.5.0`, `codecarbon==3.0.2`, `shap`, `matplotlib`, `numpy`, `torch`
- Install via:
  ```bash
  conda create -n fastai_env python=3.11
  conda activate fastai_env
  pip install fastai pandas scikit-learn==1.5.0 codecarbon==3.0.2 shap matplotlib numpy torch
