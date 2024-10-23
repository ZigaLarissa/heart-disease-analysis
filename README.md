# Heart Disease Analysis

This repository contains an analysis of heart disease data using Gaussian Mixture Models (GMM) for clustering. The goal of the analysis is to identify distinct clusters of individuals based on several health-related features and to understand the associated heart disease risk factors in each group.

## Repository Structure

- **data/**: Contains the dataset in CSV format (not pushed to the repository due to size constraints).
- **model.ipynb**: The Jupyter notebook where the analysis was conducted, including data preprocessing, model training, and clustering analysis.
- **README.md**: This file, providing an overview of the repository and the analysis.
- **.gitignore**: Specifies files and directories that should be ignored by Git, such as `.venv` and large dataset files.

## Analysis Overview

The dataset contains various health attributes, such as age, cholesterol levels, maximum heart rate, and ST depression, which are commonly used to assess heart disease risk.

### Key Steps in the Analysis:
1. **Data Preprocessing**: 
   - Cleaned and prepared the data for clustering, including handling missing values and scaling features.
   
2. **Dimensionality Reduction**: 
   - Used Principal Component Analysis (PCA) and t-SNE for visualizing the data in lower dimensions while preserving important patterns.
   
3. **Clustering Using Gaussian Mixture Models (GMM)**: 
   - Applied GMM to segment individuals into three clusters based on their health features.
   
4. **Cluster Interpretation**:
   - Analyzed the characteristics of each cluster to understand the differences in heart disease risk. Cluster 0 represents a younger, healthier population; Cluster 1 shows the highest risk of heart disease, and Cluster 2 has moderate risks.

### Results Summary:
- **Cluster 0**: Healthiest group, younger individuals with low cholesterol and no signs of heart disease.
- **Cluster 1**: Highest risk group, older individuals with elevated cholesterol, ischemia (ST depression), and a high occurrence of heart disease.
- **Cluster 2**: Intermediate risk group with moderate cholesterol and heart disease risk.

## Requirements
- Python 3.x
- Jupyter Notebook
- Required Python libraries: `pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn`

> Note: The virtual environment (`.venv`) and dataset are not included in the repository due to size constraints.

## How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/heart-disease-analysis.git
   ```
2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Open `model.ipynb` in Jupyter Notebook to explore the analysis.

## Conclusion
This analysis helps to categorize individuals into distinct groups based on their health features and assess their relative risk for heart disease. The GMM clustering provides a meaningful way to interpret and potentially target health interventions for different population segments.