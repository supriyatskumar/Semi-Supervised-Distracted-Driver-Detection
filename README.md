# Semi-Supervised-Distracted-Driver-Detection

## Problem Statement
Distracted driving is defined as any activity that takes away your attention from driving whether it be talking on a cell phone, texting, operating a radio, eating, or talking to a passenger. In 2018, there were 2841 deaths and around 400,000 people in the United States injured as a result of crashes involving distracted drivers. [1]

This project is to classify different forms of distracted driving using 2D dashboard images in a semi-supervised approach.

[1] “Distracted Driving.” NHTSA, 6 Mar. 2020, www.nhtsa.gov/risky-driving/distracted-driving.

### Use Case
* The trained model can be used by OEMs to improve auto safety.
* The semi-supervised image classification reduces the cost of collecting expensive labelled data.

## Dataset
The dataset is from State-Farm and published at https://www.kaggle.com/c/state-farm-distracted-driver-detection/data<br />
There are 22.4 K labelled and 79.7 K unlabeled samples. It consists of images of driver doing 1 of 10 actions listed below.<br />
10 classes(driver actions):
1. safe driving
2. texting - right
3. talking on the phone - right
4. texting - left
5. talking on the phone - left
6. operating the radio
7. drinking
8. reaching behind
9. hair and makeup
10. talking to passenger


## Machine Learning Problem Statement 
This is a multi-class image classification problem. Given the labelled and unlabelled 2D images, classify an image into one of 10 classes to identify driver distraction.

## Approach
In this project a Semi-supervised Generative Adversarial Network (SGAN) is used to utilize the available large set of unlabeled data samples along with labeled data to train the model.<br />
SGAN: is a modified version of GAN architecture. It trains a supervised discriminator, unsupervised discriminator and a generator model at the same time.<br />
* Supervised discriminator: Trained using real images with labels to predict the class labels<br />
* Unsupervised discriminator: Trained using unlabeled real images and generated fake images. This is similar to traditional GAN, which is used to predict real or fake sample.

## Evaluation Metric (KPI)
Accuracy

## Result
This project successfully builds a Semi-supervised GAN based model to classify distracted driver images into 10 classes, using just ~15000 labeled images and 40000 unlabeled images. The experimental results show that Semi-supervised approach yields an evaluation accuracy of 94.7%.
