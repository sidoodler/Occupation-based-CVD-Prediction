# Occupational Correlation & Predictive Modeling for Cardiovascular Disease (2015-2021)
## Project Overview
This project investigates the longitudinal relationship between occupational categories and cardiovascular health status using health survey data spanning six years. Beyond exploratory analysis, the repository implements a predictive pipeline to assess CVD risk using various machine learning architectures, including traditional statistical models and neural networks.

A key challenge addressed in this project is class imbalance, handled through synthetic data generation using Generative Adversarial Networks (GANs) and Gaussian Copula methods.

**Technical Stack**

Language: Python

Data Manipulation: pandas, numpy

Machine Learning: scikit-learn, Keras (Neural Networks), sdv (Synthetic Data Vault)

Visualization: seaborn, matplotlib

## Project Architecture
**1. Exploratory Data Analysis (EDA)**

File: Occupation_CVD_analysis.ipynb

Analyzes 6 years of historical data (2015–2021).

Maps correlations between specific industries/work categories and cardiovascular attributes.

Identifies trends in health outcomes across different occupational sectors.

**2. Data Preprocessing & Feature Engineering**

File: Main.ipynb

Merges 2020 and 2021 datasets for a robust contemporary baseline.

Implements data cleaning, normalization, and encoding.

Feature Selection: Utilizes statistical methods to extract the Top 25 features to optimize model performance and reduce dimensionality.

**3. Handling Data Imbalance (GANs)**

File: GANs.ipynb

Addresses the scarcity of CVD-positive cases in the raw data.

Methodology: Employs Gaussian Copula and GAN-based synthesis via the sdv library to generate high-fidelity synthetic samples, ensuring a balanced distribution for training.

**4. Predictive Modeling & Evaluation**

Files: DataModelling_Full_Detailed.ipynb, DataModelling_Synthetic_Data.ipynb, etc.
Comprehensive benchmarking of four core architectures:

Logistic Regression: Baseline statistical modeling.

Random Forest: Ensemble learning for feature importance.

Support Vector Machines (SVM): High-dimensional classification.

Neural Networks: Deep learning approach for non-linear pattern recognition.

## Data Setup

The datasets required for these notebooks are provided in compressed format.

Unzip other_data.zip and other_data_2.zip.

Ensure the .csv files are placed in the root directory or update the file paths within the notebooks.

Primary Data Sources:

2015.csv through 2021.csv (Yearly survey data)

adult20.csv / adult21.csv (Detailed 2020-21 datasets)

synthetic_dataGAN.csv / synthetic_dataGC.csv (Model-generated data)
