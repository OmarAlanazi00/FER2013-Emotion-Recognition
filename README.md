# Real-Time Facial Expression Recognition

## Project Overview

This project uses Computer Vision and Deep Learning to recognize facial expressions from images and live webcam video. It compares three deep learning approaches to identify the best-performing model for facial expression classification.

## Problem Description

The goal of this project is to classify facial expressions into seven categories:

- Angry
- Disgust
- Fear
- Happy
- Neutral
- Sad
- Surprise

The system detects faces using OpenCV and predicts facial expressions using a trained deep learning model.

## Dataset & Models Used

**Dataset:** FER2013 (Facial Expression Recognition 2013)

The dataset contains facial expression images divided into training and testing sets. The training data was further divided into training and validation sets.

Three models were implemented:

1. **CNN From Scratch:** A convolutional neural network trained from the beginning.
2. **Transfer Learning:** A pretrained ResNet18 model with a modified classification layer.
3. **Fine-Tuning:** A ResNet18 model with selected layers unfrozen for further training.

## Workflow / Architecture

1. Load and preprocess the FER2013 dataset.
2. Split the data into training, validation, and testing sets.
3. Apply image augmentation.
4. Train a CNN model from scratch.
5. Apply Transfer Learning using ResNet18.
6. Fine-tune selected ResNet18 layers.
7. Evaluate and compare the three models.
8. Export the fine-tuned ResNet18 model to ONNX.
9. Use OpenCV for face detection and real-time facial expression prediction.

## Results & Evaluation

The models were evaluated using the following metrics:

- Accuracy
- Precision
- Recall
- F1-Score

The fine-tuned ResNet18 achieved the best overall performance compared to CNN From Scratch and Transfer Learning.

The final model was also used for real-time facial expression recognition through a webcam, displaying a bounding box around the face and the predicted expression.

## Technologies Used

- Python
- PyTorch
- Torchvision
- OpenCV
- ONNX Runtime
- NumPy
- Matplotlib
- Scikit-learn
- Google Colab

## Future Improvements

- Improve accuracy through additional training and hyperparameter tuning.
- Improve prediction performance under different lighting conditions.
- Improve real-time detection speed.
- Test the model on more diverse facial expressions.

## SDAIA Academy GitHub Repository

https://github.com/OmarAlanazi00/FER2013-Emotion-Recognition
