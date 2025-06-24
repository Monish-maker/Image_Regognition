# 😊😢 Happy-Sad Image Classifier using CNN (TensorFlow + OpenCV)

This project is a Convolutional Neural Network (CNN) based image classification system that identifies whether a given face image is **Happy** or **Sad**. It uses TensorFlow for model building and training, and OpenCV for image processing — all run through Google Colab and Google Drive.

---

## 📂 Project Highlights

- Loads images from Google Drive
- Preprocesses and normalizes input images
- Builds a CNN with multiple Conv2D and MaxPooling layers
- Trains on labeled data (`happy_people/`, `sad_people/`)
- Evaluates with Precision, Recall, Accuracy
- Predicts custom images
- Saves trained model (`.h5` format)

---

## 🛠️ Tech Used

- Python
- TensorFlow / Keras
- OpenCV
- NumPy
- Matplotlib
- Google Colab
- Google Drive

---

## 📁 Dataset Structure (in Google Drive)

/DataSet(YT)/
├── happy_people/
│ ├── happy1.jpg
│ └── ...
└── sad_people/
├── sad1.jpg
└── ...

---

## 🧠 Model Architecture

- `Conv2D` → `ReLU` → `MaxPooling2D`
- Repeated 3 times with 16, 32, 16 filters
- `Flatten` → `Dense(256)` → `Dense(1)` with Sigmoid
- Binary classification using `BinaryCrossentropy` loss
- Optimized using Adam

---

## 📊 Training Summary

- Trained for **20 epochs**
- Validation using `val_loss`, `val_accuracy`
- TensorBoard used for logging (optional)

---

## 📈 Evaluation

Model evaluated on test set using:
- `Precision`
- `Recall`
- `Binary Accuracy`

---

## 🔍 Sample Prediction

Upload a face image → Get prediction:
The image is a Happy Image

or
The image is a Sad Image

---

## 💾 Model File & Dataset

Due to GitHub file size limits, the trained model and dataset are hosted on Google Drive:

📦 [Download Trained Model (.h5)](https://drive.google.com/file/d/1JzT6s3NO-0OTUED2EbKLNG67DePhk2MN/view?usp=sharing)

📁 [Download Dataset Folder](https://drive.google.com/drive/folders/1gi_7uLeM0sIzbp5l5VrSz6jnHRPe1a10?usp=sharing)
