# KaNCD: Knowledge-aware Neural Cognitive Diagnosis Model

This notebook demonstrates an implementation of **KaNCD (Knowledge-aware Neural Cognitive Diagnosis Model)** using the public **ASSISTments 2009–2010** dataset  
(https://sites.google.com/site/assistmentsdata/home/2009-2010-assistment-data).

KaNCD belongs to the family of **Cognitive Diagnosis Models (CDM)**, which aim to estimate students’ latent knowledge levels across multiple skills based on their question–response interactions.

---

## 📘 Overview
KaNCD combines the interpretability of classical CDMs with the representational power of **neural networks**, enabling the model to capture complex dependencies between skills.  
This notebook provides a complete pipeline, from preprocessing to model training and evaluation using the following metrics:

- **AUC (Area Under the Curve)**
- **Accuracy (ACC)**
- **POMDP-based Reward**, as an indicator of the model’s efficiency in representing student performance.

---

## 🧠 Dataset
The **ASSISTments 2009–2010** dataset is one of the most widely used benchmarks in educational data mining and cognitive diagnosis research.  
It includes:
- Student–problem interaction records  
- Correct/incorrect response labels  
- A **Q-matrix** mapping items to skills
- > [ASSISTments 2009-2010](https://sites.google.com/site/assistmentsdata/home/2009-2010-assistment-data)


---

## 📊 Evaluation Results
| Metric | Score |
|:-------|:------:|
| AUC | **0.7410** |
| ACC | **0.7503** |
| POMDP Reward | **0.792** |

---

## 💡 Recommendation
It is recommended to run this notebook in **Google Colab** for easier environment setup and GPU acceleration.  
Make sure to install dependencies such as `educdm` before executing the cells.

---

## 📁 Notebook Structure
- **Data Loading & Preprocessing**  
  Prepare the ASSISTments dataset and Q-matrix.  
- **Model Initialization**  
  Build and configure the KaNCD architecture.  
- **Training Loop**  
  Train the model using student–item interaction data.  
- **Evaluation**  
  Compute AUC, ACC, and POMDP-based reward metrics.  
- **Visualization**  
  Display results and performance across folds.

---

© 2025 Ridho — Example implementation for research and experimentation purposes.
