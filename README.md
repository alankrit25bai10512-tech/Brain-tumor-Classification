# Brain Tumor Classification 

## 📋 Overview of the Project
This project is a Deep Learning application designed to classify Brain Tumor MRI scans into specific categories. Utilizing the power of Transfer Learning, the project compares the performance of two well-known Pre-trained models: **VGG16** and **ResNet50**.

 The primary goal is to automate the detection process and assist medical diagnostics by categorizing MRI images into four distinct classes based on the presence and type of tumor i.e glioma tumor, meningioma tumor, no tumor, pituitary tumor.

## ✨ Features
* **Data Preprocessing & Augmentation:** Implements Image Data Generator for rescaling, rotation, width/height shifting, zooming, and horizontal flipping to prevent overfitting.
* **Pre-Trained Model Training:** Utilizes pre-trained weights from VGG16 and ResNet50 models, adapting them for this specific classification task.
* **Multi-Class Classification:** Capable of classifying images into 4 categories:
    * Glioma Tumor
    * Meningioma Tumor
    * Pituitary Tumor
    * No Tumor
* **Model Comparison:** Trains two separate models to compare accuracy and loss performance.
* **Visualization:** Generates comparative plots for Training Accuracy and Validation Accuracy.

## 🛠 Technologies & Tools Used
* **Language:** Python 
* **Deep Learning Framework:** TensorFlow / Keras
* **Environment:** Google Collab
* **Data Processing:** NumPy, OS
* **Visualization:** Matplotlib



# Dataset Overview
The dataset is split into separate folders for Training and Testing which consists of brain MRI images classified into four categories:
## **1) Training**
- Glioma Tumor
- Meningioma Tumor
- Pituitary Tumor
- No Tumor
## **2) Testing**
- Glioma Tumor
- Meningioma Tumor
- Pituitary Tumor
- No Tumor


## 🚀Steps to Install & Run the Project

Since this project is built in a Jupyter Notebook (specifically optimized for Google Collab), follow these steps:

## **1) Prerequisites:**

- A Google Account.

- The Brain Tumor dataset zipped (Brain-tumor-classification.zip).

## **2) Setup Google Drive:**


- Upload your Brain-tumor-classification.zip file to your Google Drive.

 * **Note:** Ensure the path in the code matches your upload location (Default in code: /content/drive/MyDrive/Brain-tumor-classification.zip).

## **3) Open the Project:**

- Upload Vithyarthi Project.ipynb(name of your project) to Google Colab.

## **4) Run the Notebook:**

* **Mount Drive:** Run the first cell to mount your Google Drive. You will be asked to authorize access.

 * **Unzip Data:** Run the second cell to extract the dataset into the Colab runtime environment.

 * **Execute cells:** Run the remaining cells sequentially to process data, build models, train, and visualize results.

## 🧪 Instructions for Testing & Evaluation
The project includes specific cells for evaluating the performance of the models after training.

## 1) Training:

* The notebook automatically trains VGG16 for 20 epochs and ResNet50 for 30 epochs.

* Wait for the training cells to complete.

## 2) Visualization:

* Locate the cell containing plt.plot(...). Run this to generate a graph comparing the training and validation accuracy of both models.

## 3) Evaluation:

* Scroll to the final code cells.

* **Run the cell for vgg  model:** vgg_model.evaluate(val_generator) to see the final Loss and Accuracy for VGG16.

* **Run the cell for resnet model:** resnet_model.evaluate(val_generator) to see the final Loss and Accuracy for ResNet50.
