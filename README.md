# Image Processing and Classification Pipeline

An end-to-end Python image processing, augmentation, and machine learning classification pipeline implemented in Google Colab using OpenCV and Scikit-Learn.

## 📌 Project Overview
This repository contains a complete laboratory assignment implementing a robust computer vision workflow. The pipeline automatically reads raw image data from Google Drive, applies standard preprocessing and augmentation techniques, extracts features, and trains a Support Vector Machine (SVM) classifier to categorize images.

---

## 🛠️ Required Tasks & Implementation Steps

1. **Google Drive Mounting:** Automatically connects Google Colab to Google Drive to access the dataset.
2. **Batch Image Reading:** Loops through class directories (`Class_0`, `Class_1`) to read images automatically.
3. **Image Resizing:** Resizes every image to a uniform standard of $128 \times 128$ pixels.
4. **Grayscale Conversion:** Converts RGB images into single-channel grayscale format.
5. **Gaussian Filtering:** Applies a $5 \times 5$ Gaussian Blur kernel to reduce image noise.
6. **Histogram Equalization:** Enhances global image contrast.
7. **Normalization:** Scales pixel intensity values to the range $[0, 1]$.
8. **Edge Detection:** Extracts sharp structural boundaries using the **Canny Edge Detection** algorithm.
9. **Image Augmentation:** Generates synthetic variations using:
   * Horizontal Flip
   * Random Rotation
   * Brightness Adjustment
10. **Dataset Preparation:** Flattens processed images into NumPy arrays (`X`) and prepares corresponding labels (`y`).
11. **Train-Test Split:** Splits dataset into **80% Training Data** and **20% Testing Data**.
12. **Model Training & Evaluation:** Trains a **Support Vector Machine (SVM)** classifier and evaluates performance using Accuracy and Confusion Matrix metrics.

---

## 📊 Visualization Requirement
The pipeline includes a custom **2 x 4 Matplotlib Grid** visualization showcasing the step-by-step transformation for a selected sample image:
* Original Image $\rightarrow$ Resized $\rightarrow$ Grayscale $\rightarrow$ Gaussian Filtered $\rightarrow$ Histogram Equalized $\rightarrow$ Normalized $\rightarrow$ Canny Edge $\rightarrow$ Augmented Version.

---

## 🚀 Tech Stack & Libraries
* **Python**
* **Google Colab**
* **OpenCV (`cv2`)**
* **NumPy**
* **Scikit-Learn (`sklearn`)**
* **Matplotlib**

---

## 👨‍💻 Author
**Md Saifullah Islam Sawon**
