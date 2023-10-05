# Occupation-based-CVD-Prediction
This project analyses health survey data from 2015-21 to assess the correlation between a person’s occupation and their cardiovascular health status. It also performs predictive modelling for the risk of cardiovascular diseases. The following models are tried: Logistic regression, Random Forest, Support vector Machine, Neural Network.

Language used - Python

Libraries required to run the notebooks:
numpy, pandas, sklearn, seaborn, matplotlib, sdv, keras

Code files:
1. Occupation_CVD_analysis.ipynb - Required data files are 2015.csv, 2016.csv, 2017.csv, 2018.csv, 2020.csv, 2021.csv. This notebook contains a detailed analysis between occupation and CVD attributes across 6 years of data among various work categories, occupations and industries.

2. Main.ipynb - Required data files are adult20.csv, adult21.csv. In this notebook, we combined the 2020 and 2021 dataset and did all preprocessing needed for data modelling. Also, extracted the top 25 features as a new dataset for modelling.

3. GANs.ipynb - Required data files are finalpreprocessed_detailed.csv. Synthesised new data with CVD = 1 distribution using Gaussian Coupla method and Gaussian method using sdv library.

4. Experimented with SVM, logistic regression, neural networks and random forest models on all datasets in all of these notebooks - DataModelling_Full_Detailed.ipynb, DataModelling_Full_Detailed2.ipynb, DataModelling_Synthetic_Data.ipynb, DataModelling_data25.ipynb. 
Required data files are finalpreprocessed_detailed.csv, synthetic_dataGAN.csv, synthetic_dataGC.csv, data25_detailed.csv. 

Data files attached:
finalpreprocessed_detailed.csv, synthetic_dataGAN.csv, synthetic_dataGC.csv, data25_detailed.csv, 2015.csv, 2016.csv, 2017.csv, 2018.csv, 2020.csv, 2021.csv, adult20.csv, adult21.csv.
Unzip other_data.zip and other_data_2.zip to access these data files.
