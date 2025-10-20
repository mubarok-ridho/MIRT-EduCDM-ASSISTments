# MIRT: Multidimensional Item Response Theory Model

This notebook presents an implementation of **MIRT (Multidimensional Item Response Theory)** using the public **ASSISTments 2009–2010** dataset  
(https://sites.google.com/site/assistmentsdata/home/2009-2010-assistment-data).

MIRT is a classical **Cognitive Diagnosis and Psychometric model** designed to estimate a student’s latent abilities across multiple skills (dimensions) based on their responses to test items.

---

## 📘 Overview
Unlike traditional unidimensional IRT, **MIRT** allows each question (item) to depend on multiple latent traits or skills simultaneously.  
This enables a richer representation of student knowledge and provides better insights into their strengths and weaknesses across different cognitive dimensions.

This notebook demonstrates the end-to-end workflow — from preprocessing to training and evaluation — using standard performance metrics:

- **AUC (Area Under the Curve)**
- **Accuracy (ACC)**
- **POMDP-based Reward**, representing model efficiency and decision consistency.

---

## 🧠 Dataset
The **ASSISTments 2009–2010** dataset is used as a benchmark for evaluating the model.  
It includes:
- Student–problem interaction records  
- Binary response outcomes (correct/incorrect)  
- A **Q-matrix** mapping each item to one or more underlying skills

---

## 📊 Evaluation Results
| Metric | Score |
|:-------|:------:|
| AUC | **0.6768** |
| ACC | **0.6993** |
| POMDP Reward | **0.5291** |

---

## 💡 Recommendation
It is recommended to run this notebook in **Google Colab** for smoother setup and GPU usage.  
Make sure to install dependencies such as `educdm` and related libraries before running the notebook.

---

## 📁 Notebook Structure
- **Data Loading & Preprocessing**  
  Prepare the ASSISTments dataset and Q-matrix.  
- **Model Definition**  
  Initialize the MIRT model parameters and latent traits.  
- **Training**  
  Fit the model to student–item interaction data.  
- **Evaluation**  
  Compute AUC, ACC, and POMDP reward metrics.  
- **Visualization**  
  Display evaluation results across multiple folds.

---

© 2025 Ridho — Example implementation for research and experimentation purposes.
