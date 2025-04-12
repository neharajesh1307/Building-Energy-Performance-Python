# Building Energy Performance ML-Based Analysis (Python)

[![Python](https://img.shields.io/badge/Python-3.8+-blue?logo=python)](https://www.python.org/)
[![scikit-learn](https://img.shields.io/badge/Scikit--Learn-ML-orange?logo=scikit-learn)](https://scikit-learn.org/)
[![Models](https://img.shields.io/badge/Models-Serialized-green)]()
[![LinkedIn](https://img.shields.io/badge/Connect-Neha%20Rajesh-blue?logo=linkedin)](https://www.linkedin.com/in/neha-rajesh-/)

Analyze and predict building energy efficiency using machine learning to support sustainable investment decisions and retrofit targeting.

## Project Overview

This project applies machine learning techniques to evaluate and forecast the energy performance of residential buildings in Ireland. It leverages clustering and classification models to:
- Identify patterns in insulation and construction characteristics
- Predict CO₂ emission classes
- Support data-driven decisions for retrofitting and green investments


## Key Features

### Clustering
- K-Means and Agglomerative Clustering
- Based on U-values and year of construction
- PCA visualization of cluster segments

### Classification
- CO₂ class prediction (Low, Medium, High)
- Models: Random Forest (ensemble), Logistic Regression 
- OneHotEncoding + StandardScaler pipeline
- Feature importance analysis

### Visualizations
- Correlation heatmaps
- Distribution plots
- Confusion matrices
- PCA plots for clusters

## Project Structure

Building_Energy_Performance_Python.ipynb # Main notebook 
BER_15_Variables_Cleaned.csv # Dataset 
random_forest_model.pkl # Saved Random Forest classifier 
logistic_regression_model.pkl # Saved Logistic Regression model 
kmeans_model.pkl # Saved K-Means model 
agglomerative_model.pkl # Saved Agglomerative model 
classification_preprocessor.pkl # Preprocessing pipeline (StandardScaler + OneHotEncoder)


## Dataset Source

The dataset is based on the **Building Energy Rating (BER)** public data from the [Sustainable Energy Authority of Ireland (SEAI)](https://ndber.seai.ie/BERResearchTool/ber/search.aspx).  
Only buildings constructed from **2000 onwards** were considered to reflect modern energy regulations.


## Insights

- U-values (wall, window, roof) are critical predictors of CO₂ class
- Newer buildings generally show lower emissions
- Electricity-based heating systems are associated with better energy performance
- Agglomerative Clustering formed clearer groups than K-Means in this dataset

## How to Run

1. Clone this repository or download the zip
2. Open the notebook `Building_Energy_Performance_Python.ipynb` in Jupyter, VS Code, or Google Colab
3. Ensure all files are in the **same directory**
4. Run all notebook cells top-to-bottom

```bash
pip install pandas numpy seaborn matplotlib scikit-learn joblib


## Model Reusability
Each model and the preprocessing pipeline is saved as a .pkl file using joblib. These can be reloaded for deployment or batch inference without retraining.

## Use Cases
Government or agency dashboards to prioritize retrofit grants
Property websites to assess environmental performance
Real estate investment tools for green housing scoring


## Author

**Neha**  
MS in Business Analytics  
[LinkedIn](https://www.linkedin.com/in/neha-rajesh-/)  
[GitHub](https://github.com/neharajesh1307)
