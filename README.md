# Titanic
This is the most famous Kaggle [competition](https://www.kaggle.com/c/titanic) in which you have to use machine learning to create a model that predicts which passenger can survive the Titanic shipwreck or not. I have done a lot of data engineering and feature engineering to clean and to increase the accuracy of my models. 

I have trained 3 models :
* Logistic Regression.
* XGBClassifier.
* Random Forest.

I have also ensemble all 3 of these models together to see the results and have only used ensemble of Logistic Regression and XGBClassifier. The accuracy in all of my submission file is a minimum of 75% in Kaggle but the best one was ensemble of Logistic Regression and XGBClassifier which is the file name [hardvoting_withoutrf](https://github.com/Moddy2024/Titanic/blob/main/results/hardvotingwithoutrf_submission.csv) which got me in the top 5% of all the people in the Titanic Competetion in Kaggle. RandomForest seems to be overfitting because we don't have a very big dataset. When comparing each of the models separately Logistic Regression works better than XGBoost and Random Forest so after ensembling the best two the ensembled model works even well.



# Dataset
You can download the dataset from Kaggle or get it in this repo which I have already downloaded from Kaggle.

For the training file go [here](https://github.com/Moddy2024/Titanic/blob/main/files%20from%20kaggle/train.csv).

For the test file go [here](https://github.com/Moddy2024/Titanic/blob/main/files%20from%20kaggle/test.csv).

# Software requirements
* Numpy
* Pandas
* Seaborn
* Matplotlib
* Scikitlearn
* XGBoost


# Key Files
* [titanic-1.ipynb](https://github.com/Moddy2024/Titanic/blob/main/titanic-1.ipynb) - In this file you can see all the data engineering and the feature engineering that I have performed. After which I train the model, ensemble them and check their cross validation score.
* [results](https://github.com/Moddy2024/Titanic/tree/main/results) - All the results of the different models and ensemble are present here in csv format.
* [files from kaggle](https://github.com/Moddy2024/Titanic/tree/main/files%20from%20kaggle) - The files that are provided by Kaggle. There are three files here training,test and gender_submission.csv. We can only use the training file for training the model for the competition and predict the results using the data in the test file for submission. The gender_submission.csv is as an example of what a submission file should look like.
