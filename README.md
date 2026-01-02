# Fuzzy Enhanced Feature Engineering for Riverbank Health Prediction

**Using Attention-Based Neural Networks and Explainable AI 2.0**

![Python](https://img.shields.io/badge/Python-3.x-blue.svg)
![Framework](https://img.shields.io/badge/Framework-Scikit--Fuzzy%20%7C%20TensorFlow-orange.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)

## 📌 Project Overview

This project introduces a **Hybrid Fuzzy–Deep Learning Framework** designed to assess and predict riverbank erosion risk. Traditional monitoring methods often fail to capture the nonlinear interactions between hydrological and geomorphological factors. To address this, our solution integrates **Fuzzy Logic** for uncertainty handling with **CBAM-enhanced LSTM networks** for accurate prediction, improved by **Explainable AI (XAI)** for transparency.

[cite_start]This research was presented at the **2nd International Conference on Data Mining and Information Security (ICDMIS 2025)**[cite: 1, 2].

## 🚀 Key Novelty & Features

* [cite_start]**Hybrid Fuzzy–Deep Learning:** Integrates human-understandable fuzzy reasoning with deep learning to handle uncertain environmental data effectively[cite: 2].
* [cite_start]**Attention-Guided Feature Engineering:** Uses a **Convolutional Block Attention Module (CBAM)** to highlight critical spatiotemporal features like slope, discharge, and sediment flux[cite: 3].
* [cite_start]**Fuzzy Logic Control System:** Maps qualitative labels (e.g., "High Erosion", "Poor Habitat") to quantitative scores using triangular membership functions[cite: 30, 31].
* [cite_start]**Explainable AI 2.0:** Incorporates **DiCE-based counterfactual explanations** to interpret model decisions, providing actionable insights for policymakers[cite: 4].

## 🛠️ Methodology

The framework processes data through three main stages:

1.  **Fuzzy Logic Assessment (Current Notebook Implementation):**
    * **Inputs:** Erosion Risk Index (ERI) & River Habitat Survey (RHS).
    * **Process:** Fuzzification of input labels $\rightarrow$ Application of Fuzzy Rules $\rightarrow$ Defuzzification.
    * [cite_start]**Output:** A concrete "River Condition Score" classifying rivers as *Good*, *Ok*, or *Worst*[cite: 31, 32].

2.  **Deep Learning Prediction:**
    * Utilizes **Long Short-Term Memory (LSTM)** networks to model temporal dependencies in river data.
    * [cite_start]Enhanced with **CBAM** to focus on the most relevant features[cite: 2, 29].

3.  **Validation:**
    * [cite_start]The model is validated on a comprehensive real-world dataset of **336 rivers** with **33 attributes**[cite: 5].

## 📂 Repository Structure

* [cite_start]`river2.ipynb`: The core Jupyter Notebook containing the data preprocessing, Fuzzy Logic implementation, and visualization code[cite: 30].
* `PREPROCESSED_DATASET (2).csv`: The dataset used for analysis (ensure this is placed in the root directory).
* `final_fuzzy_river_condition_output.csv`: Generated output file with calculated river condition scores.

## 💻 Installation & Usage

### Prerequisites
Ensure you have Python installed. You will need the following libraries:

```bash
pip install pandas numpy scikit-fuzzy tqdm matplotlib seaborn
