# Facial Emotion Recognition

---

## Introduction

Facial expressions play a crucial role in human communication, offering valuable insights into an individual's emotional state. This project aims to develop a Convolutional Neural Network (CNN) model capable of recognizing and classifying facial expressions into seven categories:

- Anger
- Disgust
- Fear
- Happiness
- Sadness
- Surprise
- Neutral

## Purpose

The purpose of this project is to showcase the potential of CNNs in facial emotion recognition and highlight their applications in psychology, human-computer interaction, and security.

---

## Dataset

The dataset used in this project was obtained from the Kaggle website. It consists of approximately 37,000 well-structured grayscale images of faces, each measuring 48 × 48 pixels. Each image was labeled with one of the seven categories representing different facial emotions:

- 0: Angry
- 1: Disgust
- 2: Fear
- 3: Happy
- 4: Sad
- 5: Surprise
- 6: Neutral

[Dataset Link](https://www.kaggle.com/datasets/msambare/fer2013)

---

## Proposed Algorithm

The model architecture consists of the following components:

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
A dense layer with a SoftMax activation function, containing 7 neurons for the different classes.

---

## Implementation Details

The model was trained using 50 epochs and a batch size of 128, utilizing all the images in the training set. Hyperparameters were cross-validated to select the model with the highest accuracy. The highest accuracy was achieved at the 49th epoch, and the model was saved at that point to maintain accuracy.

---

## Training Plots

![Training Plots](https://github.com/rohan-badugula/Facial_Emotion_Recognition/assets/75232973/0d438a10-3f11-4346-84f1-4bd86905a42b)

**Accuracy:** 82% on the validation set.
**Loss:** 1.319 on the validation set.

---

## Confusion Matrix

![Confusion Matrix](https://github.com/rohan-badugula/Facial_Emotion_Recognition/assets/75232973/30356a3b-edd2-48ce-94a2-dd5ada4fc143)

---

## Individual Prediction using Web cam
![test](https://github.com/rohan-badugula/Facial_Emotion_Recognition/assets/75232973/f70ef6bd-7d6e-42cd-9efb-2b78bb682b82) ![predic](https://github.com/rohan-badugula/Facial_Emotion_Recognition/assets/75232973/1f06e66b-8717-4d81-af08-50d586cc3b89)

---

Feel free to explore the code and project repository for more details.




