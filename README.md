# Pneumonia Detection in Chest X-rays Using Deep Learning 🩻🤖

![](images/pneumonia_cover.png) <!-- Image 1: Project cover (e.g., chest X-ray with prediction overlay) -->

## 🧠 Introduction

### Why Pneumonia Detection Matters

Pneumonia is a serious respiratory condition that affects millions of people globally and is one of the leading causes of death among children under 5 and the elderly. Early and accurate diagnosis is **critical** to ensure timely treatment and save lives.

Traditionally, pneumonia is diagnosed by radiologists examining chest X-ray images. However, this process is time-consuming and prone to human error — especially in under-resourced areas with a shortage of medical professionals.

This project addresses this issue by leveraging **deep learning** to automatically detect pneumonia in chest X-ray images, potentially providing fast, accurate, and scalable diagnosis support.

---

## 🛠 Project Overview

The objective of this project was to develop a **deep learning model using Convolutional Neural Networks (CNNs)** that can classify X-ray images into two categories: **Normal** and **Pneumonia**.

The system can assist medical professionals in quickly identifying pneumonia from chest radiographs, especially in areas where access to expert radiologists is limited.

---

## 💡 Tools & Technologies Used

- **Python**
- **TensorFlow / Keras**
- **OpenCV**
- **NumPy & Pandas**
- **Matplotlib & Seaborn**
- **Google Colab / Jupyter Notebook**

---

## 🔬 Methodology

### 1️⃣ Data Collection

The dataset used was sourced from [Kaggle's Chest X-Ray Images (Pneumonia) dataset](https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia), which includes:

- 5,863 X-ray images (JPEG format)
  - 1,583 Normal
  - 4,273 Pneumonia

![](images/pneumonia_data_split.png) <!-- Image 2: Data split bar chart or pie chart -->

### 2️⃣ Data Preprocessing

- Converted all images to grayscale
- Resized images to 150x150 pixels for uniform input
- Normalized pixel values between 0 and 1
- Augmented training images using:
  - Rotation
  - Horizontal flipping
  - Zoom

### 3️⃣ Model Building

- Built a CNN architecture with multiple convolution and pooling layers
- Used `ReLU` activation and `Sigmoid` for binary classification
- Compiled with:
  - `binary_crossentropy` loss
  - `Adam` optimizer
  - Accuracy as evaluation metric

### 4️⃣ Training & Validation

- Model trained over 10 epochs with validation
- Used early stopping to prevent overfitting
- Achieved validation accuracy of **~94%**

![](images/pneumonia_model_performance.png) <!-- Image 3: Training/validation accuracy and loss graph -->

---

## 📈 Results

- The model achieved:
  - **94% Accuracy**
  - **High Precision and Recall** on pneumonia detection
- Capable of real-time diagnosis with high confidence

### Sample Prediction Output

- ✅ Prediction: Pneumonia
- 🔍 Confidence: 98.2%

---

## 🧠 Business & Social Impact

This project highlights how **AI and deep learning can support public health** by:

- Assisting radiologists in faster diagnosis
- Reducing diagnostic errors
- Providing low-cost diagnostic tools for remote areas
- Helping in screening large volumes of patients during epidemics

Incorporating such AI tools in hospitals and mobile health apps can **save lives, reduce medical costs**, and **improve access to care** in developing regions.

---

## 🚀 Future Improvements

- Train on a larger, more diverse dataset (including COVID-related cases)
- Add multi-class classification (e.g., viral vs. bacterial pneumonia)
- Deploy as a web-based diagnostic tool with Gradio or Streamlit
- Integrate with hospital systems for real-time screening

![](images/pneumonia_future_app.png) <!-- Image 4: Vision of app/tool in use -->

---

## 🙏 Acknowledgements

Special thanks to **Kaggle** for the open-source dataset and to the open-source AI community for providing tools that empower real-world healthcare solutions.

---

**Feel free to fork this repo and contribute!**
