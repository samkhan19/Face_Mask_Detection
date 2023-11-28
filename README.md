### Face Mask Detection Project
# Abstract
In response to the rapid spread of the new Coronavirus disease (COVID-19) in Wuhan, China, in December 2019, this project focuses on developing a face mask detector using the YOLO V4 deep learning algorithm. The World Health Organization (WHO) has identified face mask-wearing as a crucial preventive measure to curb the transmission of the virus. Despite the importance of wearing masks, some individuals refuse to comply. The face mask detector presented in this project aims to address this issue.

The detector has been implemented using the YOLO V4 deep learning algorithm and tested in real-time applications. The device has been successfully installed at Politeknik Negeri Batam, demonstrating accurate detection of individuals wearing or not wearing face masks, even when in motion. The proposed technique achieves a high accuracy of 98.2%, outperforming existing models such as the Retina Facemask detector.

# Introduction
Face mask detection involves determining whether a person is wearing a mask or not. It is a reverse engineering problem of face detection, a critical area in Computer Vision and Pattern Recognition. Traditional methods based on handcrafted features and machine learning algorithms faced challenges in complexity and accuracy. Recent advancements have leveraged deep convolutional neural networks (CNN) for improved performance in face detection.

# The objectives of this project include:

Developing a novel object detection method combining one-stage and two-stage detectors for real-time detection from video streams using transfer learning.
Implementing an improved affine transformation to crop facial areas from uncontrolled real-time images, addressing variations in face size, orientation, and background.
Creating an unbiased face mask dataset with a balanced ratio.
Designing a model with low memory requirements, suitable for deployment on embedded devices for surveillance.
Analysis
The performance analysis includes an evaluation of the image complexity predictor using Kendall's coefficient τ. The predictor demonstrates a remarkable correlation (τ = 0.741) between predicted and ground truth complexity scores.

# Implementation
The implementation is carried out in Python using various libraries, including TensorFlow, OpenCV, and scikit-learn. The code includes both training and testing components.

# -> Training
The model is trained using a dataset containing images of people with and without masks. Transfer learning is applied to a MobileNetV2 base model, and an additional head model is constructed for classification. The model achieves high accuracy (98.2%) and is saved for future use.

# -> Testing
The face mask detector is tested in real-time using a video stream. The face detector model and the trained mask detector model are loaded, and the system detects and classifies faces based on the presence or absence of masks.

# Results and Outcomes
The project includes visual representations of the training process, such as loss and accuracy charts. Sample outputs show the detection of individuals with and without face masks.

# Conclusion
This work presents a deep learning-based approach to detect face masks in public places, contributing to the efforts to control the spread of COVID-19. The proposed technique demonstrates high accuracy and speed, making it suitable for real-time applications. The use of transfer learning on pre-trained models and an unbiased dataset enhances the robustness of the system.
