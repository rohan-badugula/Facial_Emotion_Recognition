# Facial_Emotion_Recognition
---
---



# Introduction

Facial expressions are a crucial part of human communication, providing insight into an individual's emotional state. In this project, a Convolutional Neural Network (CNN) model was developed to recognize and classify facial expressions into seven categories:
- Anger
- Disgust
- Fear
- Happiness
- Sadness
- Surprise
- Neutral

## Purpose
The purpose of this project was to demonstrate the potential of CNNs in recognizing facial expressions and their potential applications in fields such as psychology, human-computer interaction, and security.

---
# Dataset
The dataset used in this project was sourced from the Kaggle website and consists of approximately 37,000 well-structured 48 × 48 pixel gray-scale images of faces. Each image was classified into one of the seven categories representing different facial emotions:
- 0: Angry
- 1: Disgust
- 2: Fear
- 3: Happy
- 4: Sad
- 5: Surprise
- 6: Neutral

Dataset Link: <https://www.kaggle.com/datasets/msambare/fer2013>

---

# Proposed Algorithm
The model structure is as follows:
- Convolutional Layers (4)
- Fully Connected Layers (2)
- Softmax

## Model Architecture
The model is composed of the following components:

### Convolutional Layers (4)
- Convolution
- Spatial Batch Normalization (SBN)
- ReLU activation
- Dropout
- Max Pooling

### Fully Connected Layers (2)
- Affine transformation
- Batch Normalization (BN)
- ReLU activation
- Dropout

### Softmax Layer
A dense layer with a SoftMax activation function, with 7 neurons for the classes.

---
# Implementation Details
The model was trained using 50 epochs and a batch size of 128 with all the images in the training set. Hyperparameters were cross-validated to obtain the model with the highest accuracy. The highest accuracy was achieved at the 49th epoch, and the checkpoint was set to save the model at that point to maintain the accuracy.

---
# Training Plots
![Plots](https://github.com/rohan-badugula/Facial_Emotion_Recognition/assets/75232973/0d438a10-3f11-4346-84f1-4bd86905a42b)

# Results
- **Accuracy:** 82% on the validation generator.
- **Loss:** 1.319 on the validation generator.

---
# Confusion Matrix
![Confusion_matrix](https://github.com/rohan-badugula/Facial_Emotion_Recognition/assets/75232973/30356a3b-edd2-48ce-94a2-dd5ada4fc143)

---
# Individual Prediction using Web cam
![test](https://github.com/rohan-badugula/Facial_Emotion_Recognition/assets/75232973/f70ef6bd-7d6e-42cd-9efb-2b78bb682b82)![predic](https://github.com/rohan-badugula/Facial_Emotion_Recognition/assets/75232973/1f06e66b-8717-4d81-af08-50d586cc3b89)


