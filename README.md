# 🔬 Automated Malaria Cell Classifier using CNN

### 1. Problem Definition
The project addresses the manual, time-consuming, and error-prone process of identifying malaria parasites in red blood cell images via microscopy. The objective is to automate this process to assist diagnostic accuracy and speed, especially in low-resource settings (Healthcare Theme).

### 2. Solution and Concepts Applied
This solution uses a Convolutional Neural Network (CNN) to perform binary image classification.
* **Core CV Concept:** Image Classification and Feature Extraction.
* **Model:** Custom CNN architecture with 2 Conv2D layers.
* **Dataset:** NIH Malaria Cell Images Dataset (Parasitized vs. Uninfected).
* **Techniques:** Data Augmentation (Rotation, Zoom, Shift) and Adam Optimization.

### 3. Repository Contents
| File/Directory | Description |
| :--- | :--- |
| `malaria_classifier.py` | Complete Python script for data processing, training, and evaluation. |
| `Project_Report.pdf` | Detailed project report (as required by the assignment). |
| `screenshots/` | Plots of Confusion Matrix, Accuracy Curve, and GUI demonstration. |


### 4. Setup and Execution
To run the project, follow these steps:
1.  Clone the repository.
2.  Install dependencies: `pip install tensorflow scikit-learn seaborn pandas`
3.  **Update Data Paths:** Edit the `TRAIN_DATA_DIR` and `TEST_DATA_DIR` variables in `malaria_classifier.py` to point to your local dataset folders.
4.  Run the script: `python malaria_classifier.py`


### 5. Dataset
Malaria Cell Images Dataset in Kaggle by arunava
https://www.kaggle.com/datasets/iarunava/cell-images-for-detecting-malaria
