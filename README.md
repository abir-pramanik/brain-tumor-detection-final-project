# brain-tumor-detection-final-project
This project is made with python
cat << 'EOF' > README.md
# 🧠 Brain Tumor Detection using CNN

A deep learning project built with Convolutional Neural Networks (CNNs) to classify brain MRI scans into four categories:
- Glioma Tumor
- Meningioma Tumor
- Pituitary Tumor
- No Tumor

---

## 📁 Dataset
Used the [Brain Tumor Classification (MRI)](https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset) dataset from Kaggle, which contains grayscale MRI images organized in:
- `/Training/` directory
- `/Testing/` directory

Each directory has subfolders for each tumor class.

---

## 🧪 Project Workflow
1. **Load and Preprocess Data**
2. **Normalize & Reshape Images**
3. **Build CNN Model with Keras**
4. **Train and Evaluate the Model**
5. **Predict from Uploaded Image**

---

## 🧠 CNN Architecture (Keras)
```python
model = Sequential([
    Conv2D(32, (3,3), activation='relu', input_shape=(100, 100, 1)),
    MaxPooling2D(2, 2),
    
    Conv2D(64, (3,3), activation='relu'),
    MaxPooling2D(2, 2),
    
    Flatten(),
    Dense(128, activation='relu'),
    Dense(4, activation='softmax')
])

```

### ✅ Accuracy Achieved
Training Accuracy: ~95% (varies by run)

Validation Accuracy: ~90%

---

### 🚀 Usage (Colab)

Mount your Google Drive

Load dataset from /content/drive/MyDrive/archive/

Run the notebook cells step-by-step

Upload any MRI image to test prediction

---

### 🛠️ Requirements
Python 3.x

TensorFlow / Keras

NumPy

OpenCV

Matplotlib

Google Colab

---

### 📌 Author
[Abir]

B.Tech Student

---

### How to Run and test:

1. open the code in colab or copy it wherever you wanna run it..

2. Download and upload the dataset from this repository and upload the folder after extracting on drive ,
then mount it using colab and then locate the file (both TESTING & TRAINING dataset ) .

3. Run all cells( codes ) and then choose your image from dataset u wanna test out and watch results. :)

