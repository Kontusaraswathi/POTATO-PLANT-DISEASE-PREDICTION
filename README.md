#  Potato Disease Prediction using CNN

This project uses **Deep Learning (Convolutional Neural Networks)** to classify potato leaf images into three categories:
- **Healthy**
- **Late Blight**
- **Early Blight**

The model is trained using **TensorFlow/Keras** with image augmentation to improve performance and generalization.

---

##  Project Structure

Potato_Disease_Prediction/
│── Potato/
│ ├── Train/
│ │ ├── Healthy/
│ │ ├── Late_blight/
│ │ └── Early_blight/
│ ├── Valid/
│ │ ├── Healthy/
│ │ ├── Late_blight/
│ │ └── Early_blight/
│── potato_disease_prediction.py # Main training and prediction script
│── requirements.txt # Required Python packages
│── README.md # Project documentation

---

## 📊 Dataset
- **Dataset link**:https://www.kaggle.com/datasets/rizwan123456789/potato-disease-leaf-datasetpld
- **Training Data**: 900 images belonging to 3 classes.
- **Validation Data**: 300 images belonging to 3 classes.
- Images are resized to **256x256 pixels** before feeding into the CNN.

---

##  Model Architecture

The CNN model includes:
1. **Conv2D** + **MaxPooling2D** layers for feature extraction.
2. **Flatten** layer to convert features into a 1D vector.
3. **Dense** layer with **ReLU** activation.
4. **Dropout (0.5)** for regularization.
5. **Output Dense Layer** with **Softmax** for multi-class classification.

---

##  Data Augmentation

To avoid overfitting and improve generalization:
- **Rotation**: ±20 degrees
- **Width & Height Shift**: ±20%
- **Shear**: 20%
- **Zoom**: 20%
- **Horizontal Flip**

---

##  Training Results

| Epoch | Training Accuracy | Validation Accuracy |
|-------|-------------------|---------------------|
| 1     | 35%               | 51%                 |
| 3     | 72%               | 79%                 |
| 5     | 85%               | 85%                 |

**Final Validation Accuracy:** `85.33%`  
**Final Validation Loss:** `0.33`

---

## 🚀 Installation & Usage

### Install Dependencies
```bash
pip install -r requirements.txt
The CNN model includes:
1. **Conv2D** + **MaxPooling2D** layers for feature extraction.
2. **Flatten** layer to convert features into a 1D vector.
3. **Dense** layer with **ReLU** activation.
4. **Dropout (0.5)** for regularization.
5. **Output Dense Layer** with **Softmax** for multi-class classification.

---

##  Data Augmentation

To avoid overfitting and improve generalization:
- **Rotation**: ±20 degrees
- **Width & Height Shift**: ±20%
- **Shear**: 20%
- **Zoom**: 20%
- **Horizontal Flip**

---

## Training Results

| Epoch | Training Accuracy | Validation Accuracy |
|-------|-------------------|---------------------|
| 1     | 35%               | 51%                 |
| 3     | 72%               | 79%                 |
| 5     | 85%               | 85%                 |

**Final Validation Accuracy:** `85.33%`  
**Final Validation Loss:** `0.33`

---
Installation & Usage:
pip install -r requirements.txt

