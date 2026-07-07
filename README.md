# 🏭 ASK CNN Surface Crack Detection System

**Author:** Atharva Samadhan Khairnar 

---

## 📝 Project Overview
This repository contains a complete deep learning pipeline for **Industrial Surface Crack Detection**. The objective of this project is to automate the visual inspection of manufacturing materials or infrastructure by utilizing Computer Vision. 

Instead of using pre-trained models (like ResNet or VGG), this project demonstrates the ability to build, train, and evaluate a custom **Convolutional Neural Network (CNN)** from scratch using TensorFlow and Keras. 

### ✨ Key Features of this Script:
* **Automated Data Processing:** Automatically shuffles and splits raw image folders into `train` (70%), `validation` (15%), and `test` (15%) datasets.
* **Real-time Data Augmentation:** Prevents model overfitting by applying random rotations, zooms, and shifts to the training images dynamically.
* **Advanced Callbacks:** Implements `EarlyStopping`, `ModelCheckpoint`, and `ReduceLROnPlateau` for an optimized, resource-efficient training lifecycle.
* **Comprehensive Evaluation:** Automatically generates accuracy/loss graphs, a Confusion Matrix, and a Classification Report (Precision, Recall, F1-Score).
* **Single Image Inference:** Includes a built-in function to test the trained model on a single, unseen image and visually display the result.

---

## 🧠 Technical Stack
* **Language:** Python 3.x
* **Deep Learning Framework:** TensorFlow & Keras

## 📦 Dependencies & Prerequisites
To run this project, you will need Python installed on your system along with the following external libraries:

* `tensorflow` - For building, compiling, and training the Convolutional Neural Network.
* `numpy` - For numerical operations and matrix manipulations on image arrays.
* `matplotlib` - For plotting the training/validation graphs and displaying images.
* `scikit-learn` - For generating the final Confusion Matrix and Classification Report.

*(Note: Built-in Python modules like `os`, `shutil`, and `random` are also heavily utilized for file handling and data splitting, but require no installation).*

---

## 📂 Dataset Requirements & Directory Setup
To run this project, you must provide your own dataset of images. Before executing the script, organize your project folder exactly like this:

```text
Your_Project_Folder/
│
├── 46_ASK_CNN_Surface_Crack_Detection.py
│
└── CrackDataset/               <-- You must create this folder!
    ├── Positive/               <-- Place all images WITH cracks here
    └── Negative/               <-- Place all images WITHOUT cracks here
