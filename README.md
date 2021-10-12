# Semi-Supervised-Distracted-Driver-Detection

## Problem Statement
Distracted driving is defined as any activity that takes away your attention from driving whether it be talking on a cell phone, texting, operating a radio, eating, or talking to a passenger. In 2018, there were 2841 deaths and around 400,000 people in the United States injured as a result of crashes involving distracted drivers. [1]

This project is to recognize and correctly classify different forms of distracted driving using 2D dashboard images to minimize car accidents.

[1] “Distracted Driving.” NHTSA, 6 Mar. 2020, www.nhtsa.gov/risky-driving/distracted-driving.

### Use Case
* The trained model can be used by OEMs to improve auto safety.
* semi-supervised image classification reduces the cost of collecting expensive labelled data.

## Dataset
The dataset is from State-Farm and published at https://www.kaggle.com/c/state-farm-distracted-driver-detection/data
Training set ~22.4 K and 79.7 K unlabeled test samples. It consists of images of driver doing 1 of 10 actions listed below.
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
