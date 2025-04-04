# Hand Gesture Recognition System

## Overview
This repository contains a machine learning project focused on hand gesture recognition using XGBoost. The model is trained to recognize 18 different hand gestures with an impressive 97.39% test accuracy, achieving a 3% accuracy improvement over the baseline model.

The project demonstrates the effectiveness of advanced feature engineering and hyperparameter tuning to boost model performance. It also integrates OpenCV and MediaPipe for real-time deployment and gesture recognition.

## Key Features
18 Hand Gestures Recognized: The model identifies various hand gestures, suitable for human-computer interaction applications.

15 Geometric Features: Finger-tip distances, joint angles, and palm-relative coordinates were added to capture complex spatial relationships.

Real-Time Deployment: Integrated with OpenCV and MediaPipe to run the model in real-time.

Hyperparameter Tuning: Optimized the XGBoost model using GridSearchCV to balance accuracy and prevent overfitting.

## Technical Breakthroughs
1. Advanced Feature Engineering
To improve the model’s ability to recognize hand gestures, 15 new geometric features were engineered. These features describe the spatial relationships between hand landmarks that raw coordinates alone could not capture.

2. Hyperparameter Optimization
XGBoost parameters were optimized using 7-fold GridSearchCV to find the best hyperparameter combination. This tuning process resulted in improved model generalization and accuracy.


3. Anti-Overfitting Protocol
Early Stopping: Monitored the validation loss during training to prevent overfitting.

Train/Test Splits: Maintained a strict train/validation/test split and ensured less than a 1% accuracy drop from training to test data.

4. Performance Impact
The following table highlights the model’s performance at each stage of the project:

## Version	Accuracy Improvement:

+ Baseline	94.2%	
+ Features	96.1%	+1.9%
+ Tuning	97.39%	+3.19%
