# Deep-Learning

This repository contains a few Jupyter Notebook files we have used for different purposes in our deep learning project.

data_download.ipynb: we used this notebook file to download data images. Kaggle provided csv sheets which have urls for both train and test data, and we used this notebook file, mostly based on the code on Kaggle's discussion board, to download the data through those urls.

CNN Model.ipynb: this notebook file contains a few of our initial model experiments and model results. Currently it has the most recent model structure we used and some intermediate model performance results. We will later clean up this file to include the variations of this file from our Google Cloud platform and our own computers.

Non_landmark_processing.ipynb: because many test data images do not have a landmark and we are supposed to leave those blank in our prediction file, we used this notebook file to complete this step. Based on the confidence of the predictions, we used threshold values to decide if some test images do not have a landmark. 
