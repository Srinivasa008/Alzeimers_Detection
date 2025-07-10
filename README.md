# 🧠 Alzheimer's Detection System

A deep learning-based web application to detect Alzheimer's disease stages from MRI brain scan images using transfer learning with VGG16.

## 🚀 Features

- Classifies MRI images into 4 categories: **Mild Demented**, **Moderate Demented**, **Non-Demented**, **Very Mild Demented**
- Utilizes **VGG16** pre-trained CNN model for high accuracy
- Achieves **~85% accuracy** through transfer learning and fine-tuning
- Preprocessing with image augmentation and resizing
- Simple user interface to upload and predict brain scan images

---

## 🛠️ Tech Stack

- **Frontend**: Streamlit (or Flask, if applicable)
- **Backend**: Python, TensorFlow, Keras
- **Libraries**: NumPy, Matplotlib, OpenCV, Scikit-learn
- **Model**: VGG16 (Transfer Learning)

---

## 📂 Dataset

- **Source**: [Kaggle - Alzheimer's MRI Dataset](https://www.kaggle.com/datasets)
- Includes 4 categories:
  - Mild Demented
  - Moderate Demented
  - Non Demented
  - Very Mild Demented

---

## 🧪 Model Training

1. Preprocess images (resize to 224x224, normalize)
2. Load VGG16 (without top layers)
3. Add custom dense layers for classification
4. Compile model (Adam optimizer, categorical crossentropy)
5. Train on 80% training data, validate on 20%

---

## 📊 Results

- **Accuracy**: ~85%
- **Loss**: Reduced significantly with data augmentation and tuning
- **Confusion Matrix**: Shows good distinction between classes

---

## 📷 Screenshots

> *(Optional: Add prediction interface, accuracy plot, confusion matrix images here)*

---

## 🧑‍💻 How to Run Locally

1. Clone the repository  
   ```bash
   git clone https://github.com/yourusername/alzheimers-detection.git
   cd alzheimers-detection


Install dependencies
bash

  pip install -r requirements.txt

Run the app
  streamlit run app.py
