# Deep-Learning

This repository contains a few Jupyter Notebook files we have used for different purposes in our deep learning project.

data_download.ipynb: 

We used this notebook file to download data images. Kaggle provided csv sheets which have urls for both train and test data, and we used this notebook file, mostly based on the code on Kaggle's discussion board, to download the data through those urls.

CNN Model.ipynb: 

This notebook file contains a few of our initial model experiments and model results. Currently it has the most recent model structure we used and some intermediate model performance results.

resnet34.ipynb

This notebook file contains training processing of ResNet-34 model and corresponding model results.

DELF_filtering_I.ipynb

In this file, we first compute the average score of representative landmark features returned by DELF for each test image, and then filter out those with low average score. Intuitively, the test images with low average score won't be landmark images with high possibility.

DELF_filtering_II.ipynb

In this file, first we use DELF to extract common features with high scores from each test image and five representative images of its corresponding prediction, respectively. Then we apply RANSAC to estimate the number of line segments (inliers) for five pairs and take the average. At last, a test image will be filtered out (namely leave the prediction blank) if its average number of inliers is less than some prespecified threshold.

Non_landmark_processing.ipynb: 

Because many test data images do not have a landmark and we are supposed to leave those blank in our prediction file, we used this file to complete this step. Based on the confidence scores of the predictions, we used some threshold value to decide if some test images do not have a landmark. 
