# Rainfall-Prediction-using-XGBoost-and-SVM
The repository contains google colab notebook for rainfall prediction task.

# Description
The dataset contains 870 rows × 7 columns in a space separated manner. The columns are ‘SAM’, ‘nino’, ‘ISMR’, ‘AMO’, ‘NAO’, ‘PDO’, ‘At-nino’, ’IOD’. Here ISMR is mean monthly rainfall in Indian region. Other columns denote potential causal drivers for ISMR, which are climatic conditions in other parts of the world. The rows contain monthly data for the months ‘May’, ‘June’, ‘July’, ‘Aug’, ‘Sep’, ‘Oct’ for the years 1871-2015 (145x6=870).  E.g., The first row contains the data for May, 1871. 
ISMR can be predicted using the potential drivers, but the lags can be different. E.g., If rainfall of July is caused by the driver values of May, then the lag value will be 2. That means the predictor values of 2 months back causes the rainfall of the current month. 

Implemented Xgboost Regresssor and SVM model to predict ISMR for different lag values of the drivers and printed the true and predicted values of the ISMR for different lags in a tabular form and plotted the true values vs predicted values of ISMR in scatter plots for different lags separately. Found the best working parameter for both the models and their lag values and detrmined the most and least likely reasons causing rainfall.
