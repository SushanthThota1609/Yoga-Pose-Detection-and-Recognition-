Yoga Pose Detection and Recognition

This repository contains the implementation of a model for yoga pose detection and recognition. The project consists of three main components:

1. Yoga Pose Classification on Images
Three classifications: Warrior2 pose, T pose, and Tree pose.
Input: An image of a yoga pose.
Output: Image with the classified pose, calculated angles, and skeleton-based figure.
MediaPipe model is used for extracting keypoints from the posture detected in the image.
Skeleton-based model of the detected landmarks is demonstrated on the output image.
Angle of flexion at all the 8 detected joints is calculated.
Classification of yoga posture is performed using an if-else tree among the defined categories.
2. Yoga Pose Correction on Real-Time Videos
Development of a yoga posture coaching system.
Input: Real-Time source video, Target image.
Output: Final Score, feedback, and skeleton figure in Real-Time.
User's yoga pose is compared with the target image, providing feedback on the screen suggesting possible changes required.
Final score is dependent on p_score (considering the landmarks of the skeleton-based model) and a_score (considering angle of flexion at the joints).
3. Prediction Model
Detection of keypoints using MediaPipe and Movenet frameworks and stored in CSV files.
Labelling of data considering 5 classifications: down-dog, warrior2, goddess, plank pose, and tree pose.
Development of prediction models using Decision Tree Regressor, Decision Tree Classifier, and Logistic Regression.
Results and Discussion:
Results with landmark detection using MediaPipe:
Decision Tree Regressor:
Accuracy: 69.7%
Recall Score: 69.5%
Precision Score: 69.4%
Decision Tree Classifier:
Accuracy: 75.8%
Recall Score: 75.6%
Precision Score: 76.7%
Logistic Regression:
Accuracy: 81.6%
Recall Score: 81.4%
Precision Score: 82.3%
Results with landmark detection using Movenet:
Decision Tree Regressor:
Accuracy: 92.03%
Recall Score: 92.40%
Precision Score: 90.21%
Decision Tree Classifier:
Accuracy: 94.02%
Recall Score: 93.01%
Precision Score: 92.10%
Logistic Regression:
Accuracy: 90.03%
Recall Score: 92.67%
Precision Score: 88.30%
