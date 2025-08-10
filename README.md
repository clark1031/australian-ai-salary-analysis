# A Predictive and Interpretive Analysis of Salary Drivers in the Australian AI Skills Landscape

**Author:** Jiansong Zhang  
**Course:** Big Data Analysis and Project (The University of Adelaide)  
**Date:** Aug 2025

---

### **1. Project Overview**

This repository contains the complete codebase and analysis for a comprehensive project on the Australian Artificial Intelligence (AI) job market. The primary goal of this study is to identify and quantify the key drivers of salary for AI-related roles in Australia, balancing predictive accuracy with model interpretability.

The project leverages a dataset of 732 Australian job postings from the "Global AI Job Market & Salary Trends 2025" dataset. A multi-phase methodology was employed, including:
-   Data Sourcing and Pre-processing
-   Exploratory Data Analysis (EDA) to uncover initial trends
-   Feature Engineering using skill clustering and one-hot encoding
-   Comparative evaluation of three regression models (Multiple Linear Regression, Ridge Regression, and Random Forest) to predict salaries
-   In-depth interpretation of model coefficients to provide actionable insights.

The key finding is that seniority level is the dominant predictor of salary, explaining approximately 75% of the variance. A standard Multiple Linear Regression model was identified as the most effective tool for this task. The final report, which details these findings and their implications, is the primary output of this work.

### **2. Repository Structure**

-   [`australian_ai_salary_analysis.ipynb`](https://github.com/clark1031/australian-ai-salary-analysis/blob/main/australian_ai_salary_analysis.ipynb): The main Jupyter/Colab notebook containing all Python code for data loading, cleaning, analysis, visualization, and modeling.
-   `README.md`: This file, providing an overview and instructions for replication.

### **3. How to Replicate the Analysis**

#### **3.1 Prerequisites**

The analysis was designed to be run in a Google Colab environment. The following core Python libraries are required and are pre-installed in Colab:
-   `pandas`
-   `numpy`
-   `matplotlib`
-   `seaborn`
-   `scikit-learn`
-   `kagglehub`

If running the notebook in a local Jupyter environment, these can be installed via pip:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn kagglehub
```

#### **3.2 Data Source**

This project uses the **Global AI Job Market & Salary Trends 2025** dataset, which is loaded directly from Kaggle.
-   **Original Source Link:** [https://www.kaggle.com/datasets/bismasajjad/global-ai-job-market-and-salary-trends-2025](https://www.kaggle.com/datasets/bismasajjad/global-ai-job-market-and-salary-trends-2025)

The raw dataset does not need to be downloaded manually, as the notebook handles this via the Kaggle API.

#### **3.3 Execution Steps**

To replicate the analysis, please follow these steps:

1.  **Prepare your Kaggle API Key:**
    -   To run the notebook, you need a Kaggle API key. Log in to your Kaggle account, go to your account settings page, and in the "API" section, click **"Create New Token"**.
    -   This will download a `kaggle.json` file to your computer.

2.  **Run the Notebook in Google Colab:**
    -   Open the [`australian_ai_salary_analysis.ipynb`](https://github.com/clark1031/australian-ai-salary-analysis/blob/main/australian_ai_salary_analysis.ipynb) notebook in Google Colab.
    -   Run the **first code cell** under "PHASE 1". It will prompt you to upload a file. Select the `kaggle.json` file you downloaded in the previous step. This will authenticate your session.
    -   Once authenticated, run the remaining cells sequentially from top to bottom. The notebook is structured to follow the 5-phase methodology, and all outputs, including tables and figures from the final report, will be generated.

### **4. Summary of Results**

The final analysis concluded that a Multiple Linear Regression model was the most effective for this task, providing an excellent balance of high predictive accuracy (R² = 0.749, MAE = $18,816) and superior interpretability. The model's coefficients were used to quantify the specific monetary value of experience levels and key technical skills in the Australian AI market.

For a detailed discussion of the results, methodology, and implications, please refer to the comprehensive final report submitted for the assignment.
