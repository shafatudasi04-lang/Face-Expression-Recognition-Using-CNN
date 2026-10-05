# Face Expression Recognition Using CNN

A deep learning project for recognizing human facial expressions using a **Convolutional Neural Network (CNN)** with **TensorFlow and Keras**.

The model classifies facial images into **seven different expressions**:

* Angry
* Disgust
* Fear
* Happy
* Neutral
* Sad
* Surprise

## 📌 Project Overview

Facial Expression Recognition is a computer vision and deep learning task that identifies human emotions from facial images.

In this project, a CNN model is trained on facial expression images. The images are converted to grayscale, resized to **48 × 48 pixels**, normalized, and augmented before being provided to the CNN model.

The trained model can predict the expression of a new facial image.

## 🎯 Objectives

* Build a CNN-based facial expression recognition system.
* Preprocess and normalize facial images.
* Apply image augmentation to improve model generalization.
* Train a deep learning model using TensorFlow and Keras.
* Evaluate the model using accuracy, loss, classification report, and confusion matrix.
* Predict facial expressions from new images.

## 🗂️ Dataset

The project uses the **Face Expression Recognition Dataset**.

The dataset contains seven expression classes:

```text
angry
disgust
fear
happy
neutral
sad
surprise
```

The dataset is organized into training and validation folders.

> The dataset itself is not included in this repository. It can be downloaded through Kaggle/KaggleHub.

## 🛠️ Technologies Used

* Python
* TensorFlow
* Keras
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* KaggleHub
* Google Colab / Jupyter Notebook

## 🧠 CNN Architecture

The model consists of multiple convolutional blocks followed by fully connected layers.

### Main Layers

* Convolutional Layers
* Batch Normalization
* ReLU Activation
* Max Pooling
* Dropout
* Flatten
* Dense Layer
* Softmax Output Layer

The final layer contains **7 neurons**, one for each facial expression class.

## 🔄 Data Preprocessing

The following preprocessing techniques are applied:

* Image resizing to **48 × 48**
* Conversion to grayscale
* Pixel normalization using `1/255`
* Random rotation
* Width and height shifting
* Zoom augmentation
* Horizontal flipping

These techniques help the model learn more robust facial features.

## ⚙️ Training Configuration

| Parameter      | Value                    |
| -------------- | ------------------------ |
| Image Size     | 48 × 48                  |
| Image Channels | 1 (Grayscale)            |
| Batch Size     | 64                       |
| Maximum Epochs | 10                       |
| Optimizer      | Adam                     |
| Learning Rate  | 0.0005                   |
| Loss Function  | Categorical Crossentropy |
| Output Classes | 7                        |

## 📊 Model Evaluation

The model is evaluated using:

* Training Accuracy
* Validation Accuracy
* Training Loss
* Validation Loss
* Classification Report
* Confusion Matrix
* Actual vs Predicted Images

These evaluation methods help analyze the performance of the CNN model for each expression class.

## 🚀 Project Workflow

```text
Dataset
   ↓
Data Preprocessing
   ↓
Image Augmentation
   ↓
Data Loading
   ↓
CNN Model Building
   ↓
Model Compilation
   ↓
Model Training
   ↓
Model Evaluation
   ↓
Predictions
   ↓
New Image Expression Recognition
```

## 💾 Model File

The trained model is saved in Keras format:

```text
face_expression_cnn.keras
```

This model can be loaded later to make predictions without retraining the CNN.

## 🔮 Future Improvements

Possible improvements include:

* Increasing the training dataset.
* Using transfer learning models.
* Applying more advanced data augmentation.
* Hyperparameter optimization.
* Training for more epochs with suitable regularization.
* Deploying the model as a web application.
* Real-time facial expression recognition using a webcam.
* Improving performance on difficult classes such as fear and disgust.

## 📁 Project Structure

```text
Face-Expression-Recognition-Using-CNN/
│
├── README.md
├── face_expression_cnn.keras
├── requirements.txt
├── Face_Expression_Recognition_CNN_Documentation.pdf
│
├── notebooks/
│   └── Face_Expression_Recognition_CNN.ipynb
│
├── results/
│   ├── accuracy.png
│   ├── loss.png
│   └── confusion_matrix.png
│
└── src/
    └── predict.py
```

## 👨‍💻 Author

**Shafaat Ullah**

Artificial Intelligence / Data Science

## 📜 License

This project is created for educational and learning purposes.
