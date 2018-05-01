# Deep-Learning

This repository contains a few Jupyter Notebook files we have used for different purposes in our deep learning project.

data_download.ipynb: 

we used this notebook file to download data images. Kaggle provided csv sheets which have urls for both train and test data, and we used this notebook file, mostly based on the code on Kaggle's discussion board, to download the data through those urls.

CNN Model.ipynb: 

this notebook file contains a few of our initial model experiments and model results. Currently it has the most recent model structure we used and some intermediate model performance results.

resnet34.ipynb

this notebook file contains training processing of ResNet-34 model and model results.

DELF_filtering1.ipynb

In this file, first we compute the average score of representative landmark features returned by DELF for each test image, and then filter out those with low average score. Intuitively, the test images with low average score won't be landmark images with high possibility.

DELF_filtering2.ipynb

In this file,  First we use DELF to extract common features with high scores from each test image and five rep- resentative images of its corresponding prediction, respec- tively. Then we apply RANSAC to estimate the number of line segments (inliers) for five pairs and take the average. At last, a test image will be filtered out (namely leave the pre- diction blank) if its average number of inliers is less than some threshold.


Non_landmark_processing.ipynb: 

because many test data images do not have a landmark and we are supposed to leave those blank in our prediction file, we used this notebook file to complete this step. Based on the confidence of the predictions, we used threshold values to decide if some test images do not have a landmark. 
