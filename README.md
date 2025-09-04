# 🤟 American Sign Language (ASL) Identification using Keras

This project focuses on classifying American Sign Language (ASL) hand gestures using a Convolutional Neural Network (CNN) built with TensorFlow and Keras. It uses the ASL image dataset from Kaggle provided by [ayuraj](https://www.kaggle.com/datasets/ayuraj/asl-dataset), and includes preprocessing steps like image blurring and edge detection to enhance model performance.

---

## 📂 Dataset

- **Source:** [ASL Dataset by ayuraj](https://www.kaggle.com/datasets/ayuraj/asl-dataset)
- **Classes:** 26 alphabets (A–Z) and 10 numbers (0-9)
- **Image Format:** `.jpg`
- **Structure:** Each letter has its own folder containing grayscale images of hands showing the respective sign.

---

## 🧪 Preprocessing Techniques

To improve model generalization and reduce noise, the following techniques are applied:

### 🔹 Blurring
- **Averaging Blur:** Smooths the image by averaging pixel values.
- **Bilateral Filter:** Reduces noise while preserving edges.

### 🔹 Edge Detection
- **Canny Edge Detection:** Detects sharp changes in intensity.
- **Prewitt Operator:** Highlights vertical and horizontal edges.

Preprocessing is done using OpenCV and applied uniformly across the dataset.

---

## 🧠 Model Architecture

The model is built using Keras Sequential API and includes:

- Convolutional layers (Conv2D)
- MaxPooling layers
- Dropout for regularization
- Flatten and Dense layers
- Softmax output for 26-class classification

### 🔧 Model Summary
- Input: Processed image (grayscale/edge-detected)
- Output: One-hot encoded letter class (A–Z)

<img width="1251" height="848" alt="image" src="https://github.com/user-attachments/assets/ee09082f-cdc8-4293-962d-754ded5379bf" />
Here is the combination of the average accuracy for each vehicle class on the CNN model.
