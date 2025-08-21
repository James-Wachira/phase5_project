# 🌍 Cropland Mapping with Machine Learning & Deep Learning

## 📌 Project Overview

This project focuses on **cropland classification in arid and semi-arid
regions** using **Sentinel satellite imagery**. The goal is to identify
cropland areas from radar (Sentinel-1) and optical (Sentinel-2) data,
leveraging both traditional machine learning (Random Forest) and deep
learning (Neural Networks).

The work is based on the **Zindi GeoAI Challenge dataset** and
demonstrates how remote sensing data can be transformed into actionable
insights for agricultural planning and monitoring.

------------------------------------------------------------------------

## 🎯 Objectives

-   Preprocess and integrate **multi-source satellite imagery**
    (Sentinel-1 & Sentinel-2).\
-   Train and evaluate **machine learning classifiers** (Random Forest,
    RandomizedSearchCV).\
-   Implement a **Neural Network model** to handle class imbalance.\
-   Generate **business-driven recommendations** for agricultural
    resource allocation.\
-   Provide a reproducible workflow for cropland mapping.

------------------------------------------------------------------------

## 📂 Project Structure

    ├── cropland_mapping_v2.ipynb   # Main analysis notebook
    ├── data/                       # Input datasets (not included in repo)
    │   ├── Train/                  # Training imagery
    │   ├── Test.csv                # Test set (without target)
    │   ├── Sentinel1.csv           # Radar features
    │   ├── Sentinel2.csv           # Optical features
    │   └── sentiment2/             # Additional test dataset
    ├── models/                     # Saved models (optional)
    ├── outputs/                    # Predictions, evaluation metrics, visualizations
    └── README.md                   # Project documentation

------------------------------------------------------------------------

## ⚙️ Methodology

1.  **Data Preparation**
    -   Preprocessing Sentinel-1 & Sentinel-2 data\
    -   Handling missing values, scaling, and feature engineering
2.  **Modeling**
    -   Baseline: Random Forest Classifier with hyperparameter tuning
        (`RandomizedSearchCV`)\
    -   Neural Network: Implemented with undersampling to address class
        imbalance
3.  **Evaluation**
    -   Accuracy: **\~92%** on validation\
    -   False Positives/Negatives: \~7k each on test set
4.  **Business Recommendations**
    -   **Targeted Field Verification**: Focus ground inspections on
        high-confidence cropland areas.\
    -   **Optimized Resource Allocation**: Prioritize irrigation,
        fertilizer, and pest control investments.\
    -   **Early-Warning for Land-Use Changes**: Quarterly monitoring to
        detect land degradation or encroachment.

------------------------------------------------------------------------

## 📊 Key Results

-   Achieved **92% classification accuracy** in distinguishing cropland
    vs non-cropland.\
-   Demonstrated the value of **combining radar + optical data**.\
-   Validated **Random Forest + Neural Network** approaches for
    geospatial classification.

------------------------------------------------------------------------

## 🚀 Next Steps

-   Extend models with **transformer-based architectures** for satellite
    imagery.\
-   Incorporate **time-series analysis** to track cropland dynamics.\
-   Deploy model as an **interactive dashboard** for policymakers and
    stakeholders.

------------------------------------------------------------------------

## 🛠️ Tech Stack

-   **Python** (NumPy, Pandas, Scikit-learn, TensorFlow/Keras)\
-   **Geospatial Libraries**: Rasterio, GDAL (optional)\
-   **Visualization**: Matplotlib, Seaborn\
-   **Tools**: Jupyter Notebook, GitHub for version control

------------------------------------------------------------------------

## 👤 Author

**James Wachira**
Data Scientist \ Remote Sensing & Machine Learning Enthusiast
