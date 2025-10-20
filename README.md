# KaNCD: Kolmogorov–Arnold Neural Cognitive Diagnosis Model

This notebook demonstrates an implementation of **KaNCD (Kolmogorov–Arnold Neural Cognitive Diagnosis Model)** using the public **ASSISTments 2009–2010** dataset  
(https://sites.google.com/site/assistmentsdata/home/2009-2010-assistment-data).

KaNCD belongs to the family of **Cognitive Diagnosis Models (CDM)**, which aim to estimate students’ latent knowledge states across multiple skills based on their question–response interactions.

---

## 📘 Overview
KaNCD leverages the **Kolmogorov–Arnold representation theorem** to model complex non-linear relationships between latent skills and student performance.  
Compared to traditional CDMs, KaNCD introduces a neural architecture that enhances the model’s ability to capture multi-skill dependencies while maintaining interpretability.

This notebook provides a full pipeline—from data preprocessing to model training and evaluation—using the following key metrics:

- **AUC (Area Under the Curve)**
- **Accuracy (ACC)**
- **POMDP-based Reward**, as an efficiency indicator of the model’s performance.

---

## 🧠 Dataset
The **ASSISTments 2009–2010** dataset is a widely used benchmark in educational data mining and cognitive diagnosis research.  
> [ASSISTments 2009-2010](https://sites.google.com/site/assistmentsdata/home/2009-2010-assistment-data)

---

## 📊 Evaluation Results
| Metric | Score |
|:-------|:------:|
| AUC | **0.7410** |
| ACC | **0.7503** |
| POMDP Reward | **0.792** |

---

## 💡 Recommendation
It is recommended to run this notebook in **Google Colab** for convenient setup and GPU acceleration.  
Ensure all required dependencies (e.g., `educdm`) are properly installed before execution.

---

## 📁 Notebook Structure
- **Data Loading & Preprocessing**  
  Prepare the ASSISTments dataset and corresponding Q-matrix.  
- **Model Initialization**  
  Build and configure the KaNCD architecture based on Kolmogorov–Arnold representation.  
- **Training Process**  
  Train the model using student–item interaction data.  
- **Evaluation**  
  Compute AUC, ACC, and POMDP reward metrics.  
- **Visualization**  
  Display results and cross-fold performance metrics.

---

© 2025 Ridho — Example implementation for research and experimentation purposes.
