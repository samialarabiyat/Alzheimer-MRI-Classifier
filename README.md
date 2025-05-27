# 🧠 Alzheimer MRI Classifier
A deep learning model that classifies Alzheimer's disease stages from brain MRI scans and visualizes model attention using Grad-CAM. Built with TensorFlow and Keras.


A deep learning model that classifies brain MRI scans into 4 stages of Alzheimer's disease and highlights the most relevant brain regions using Grad-CAM visualizations.

---

## 🔍 Features

- ✅ CNN model built using **Keras Functional API**
- ✅ Classification into 4 stages of Alzheimer’s disease
- ✅ **Grad-CAM** heatmaps to visualize model decisions
- ✅ Evaluation using **Confusion Matrix** and **Classification Report**

---

## 📁 Dataset

The dataset is provided in CSV format and contains MRI images encoded as byte strings:

- `alzheimer_train.csv`
- `alzheimer_test.csv`

Each row contains:
- An image in byte format
- A label (0, 1, 2, or 3)

---

## 🧪 Model Architecture

```text
Input (128x128 grayscale)
→ Conv2D (32 filters)
→ MaxPooling2D
→ Conv2D (64 filters)
→ MaxPooling2D
→ Flatten
→ Dense (128)
→ Dropout
→ Output Layer (Softmax, 4 classes)
Built using TensorFlow / Keras.

📊 Results
Achieved ~97% test accuracy 🎯

Confusion matrix and classification report included

Visual explanations using Grad-CAM

🖼 Grad-CAM Example
Visualizing where the model focuses in misclassified images:


🚀 How to Use
Clone the repo or upload the code to your environment (e.g. Colab or Jupyter)

Make sure you have the dataset files:

alzheimer_train.csv

alzheimer_test.csv

Run the notebook alzheimer_cnn_gradcam.ipynb

Visual outputs will be generated automatically

Libraries used:

tensorflow

numpy

pandas

matplotlib

opencv-python

seaborn

scikit-learn

tqdm

✍️ Author
Built with ❤️ by Sami (Neon AI Team)

🧠 Future Ideas
Try Transfer Learning with MobileNet

Add Streamlit web interface

Export trained model to ONNX or TensorFlow Lite


