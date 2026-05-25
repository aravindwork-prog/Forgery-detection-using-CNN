#  Handwritten Signature Forgery Detection Using CNN

A deep learning-based handwritten signature forgery detection system using a **Convolutional Neural Network (CNN)** to classify signatures as **genuine** or **forged**.

This project applies computer vision and deep learning techniques to automate signature verification and reduce manual authentication effort.

---

##  Project Overview

Signature verification is widely used in banking, legal documentation, and identity authentication. However, handwritten signatures are vulnerable to forgery.

This project uses a **Convolutional Neural Network (CNN)** to analyze signature images and classify them into:

- ✅ **Genuine Signature**
- ❌ **Forged Signature**

The model learns visual patterns from handwritten signatures and achieves high classification accuracy.

---

##  Features

- Signature image classification using **CNN**
- Data preprocessing and augmentation
- Exploratory Data Analysis (EDA)
- Model training and evaluation
- Performance visualization
- Signature prediction on new images
- Binary classification (**Real vs Forged**)

---

##  Model Architecture

The project uses a custom **Convolutional Neural Network (CNN)** built with TensorFlow/Keras.

### CNN Layers

- **Conv2D (16 filters)** + ReLU
- **MaxPooling2D**
- **Dropout (0.25)**

- **Conv2D (32 filters)** + ReLU
- **MaxPooling2D**
- **Dropout (0.25)**

- **Conv2D (64 filters)** + ReLU
- **MaxPooling2D**
- **Dropout (0.25)**

- **Conv2D (128 filters)** + ReLU
- **MaxPooling2D**
- **Dropout (0.25)**

### Fully Connected Layers

- **Flatten**
- **Dense (128 units)** + ReLU
- **Batch Normalization**
- **Dropout (0.25)**
- **Dense (1 unit)** + Sigmoid activation

### Compilation

```python
loss = 'binary_crossentropy'
optimizer = 'adam'
metrics = ['accuracy']
