# Customer-Segmentation Project (Adult dataset)
Overview:
This repository contains a project on customer segmentation using the Adult dataset. The goal of the project is to classify the customers based on income per annum, to predict which class of income they fall into using the demographic and socio-economic characteristics of individuals to identify meaningful customer segments. Customer segmentation is a crucial aspect of marketing and business strategy, helping businesses tailor their products and services to different customer groups. 
Dataset:
The dataset used in this project is the Adult dataset from the UCI Machine Learning Repository. It includes various features such as age, education, occupation, marital status, and income, among others. The dataset is preprocessed and cleaned to ensure data quality and relevance to the segmentation analysis.
## Project description:
This project is divided into two parts
  1. Data Pre-processing(Data Cleaning).
  2. Model Fitting.
   1. Data Pre-processing:
   In Data Pre-processing we clean the dataset, where we deal with outliers, missing values, duplicates, incorrect column names, scale or metrics used in the numeric columns, datattypes of the column attributes etc. After dealing with the above factors we store the cleaned dataset for the next stpe which is model fitting.
2. Model fitting:
  In Model fitting we load the dataset into our environment, since this is a classification problem we check whether we have any imbalance in the classes of our target variable which might cause a bias in our model which in turn effects the performance of our model. We correct the imbalance, then proceed with the model fitting. Here the target variable is income per annum, which is classified into two categories. 
  1. Income above >$104k per annum.
  2. Income below are equal to <=$104k per annum.
  This prediction based on various features and classification is done using mulitple ML models
  1. Logistic Regression.
  2. Random Forest Classifier.
  3. Support Vector Machine(SVM).
  4. XGBoost(XGB).
The performance of these models is evaluated based on precision, recall and F1-Score. Usually the metric on which these models are evaluated depends on the data, and the costs allotted to False Positives and False Negatives, since we want to optimize False negatives it's ideal to choose recall as out evaluation metric. 
After the evaluation we can still improve the performance of these models using Hyperparameter tuning, as we know every model has some parameters which with a slightest change can effect the performance of our model. So we performed Random Search and then Grid Search to exhaustively search for the best parameters. Then Random Forest performed better than all other models when considered recall as our evaluation metric.

## Project Structure
The repository is organized as follows:

data: Contains the preprocessed datasets.
notebooks: Jupyter notebooks used for data exploration, preprocessing, and segmentation analysis.
docs: Documentation files, including this README.

## Results
The project results, including identified customer segments and any visualizations, are documented in the notebooks.

## Contributing
Feel free to contribute to this project by opening issues or submitting pull requests. Your input is valuable, and collaboration is encouraged.

## Acknowledgments
The Adult dataset is sourced from the UCI Machine Learning Repository.
Thanks to the open-source community for various libraries and tools used in this project.

### Contact
For any questions or feedback, please contact [bs441@usf.edu].

Happy Data Exploration!!

