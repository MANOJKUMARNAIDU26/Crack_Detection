# 🧱 Crack Detection AI using Deep Learning

An AI-powered crack detection system that automatically identifies structural cracks from images using a deep learning segmentation model. The application provides crack localization, severity assessment, and an interactive web interface for real-time analysis.

---

## 📌 Overview

Structural health monitoring is essential for ensuring the safety of buildings, bridges, roads, and other civil infrastructure. Manual inspection is often time-consuming, expensive, and prone to human error.

This project leverages a **U-Net deep learning model with a ResNet50 encoder** to accurately segment cracks from images. A **Streamlit** application allows users to upload images and receive instant predictions, including crack percentage and severity classification.

---

## ✨ Features

- AI-based crack detection using Deep Learning
- Pixel-wise crack segmentation
- Automatic crack severity estimation
- Real-time image analysis
- Interactive Streamlit dashboard
- Crack overlay visualization
- Simple and user-friendly interface

---

## 🛠️ Tech Stack

### Languages
- Python

### Deep Learning
- TensorFlow
- Keras
- U-Net
- ResNet50

### Computer Vision
- OpenCV
- NumPy

### Visualization
- Matplotlib

### Deployment
- Streamlit

---

## 📂 Project Structure

```
crack-detection-ai/
│
├── app.py                     # Streamlit application
├── predict.py                 # Prediction pipeline
├── notebook/
│   └── crack_risk_analysis.ipynb
├── requirements.txt
├── crack_pretrained_model.keras
├── README.md
└── .gitignore
```

---

## 🧠 Model Architecture

- Model: U-Net
- Encoder: ResNet50 (Pretrained)
- Input Size: 256 × 256 × 3
- Output: Binary Crack Segmentation Mask
- Activation: Sigmoid

### Loss Function

- Binary Cross Entropy
- Dice Loss

### Evaluation Metrics

- Dice Coefficient
- Intersection over Union (IoU)

---

## ⚙️ Workflow

1. Upload an image through the Streamlit interface.
2. Resize the image to **256 × 256**.
3. Apply ResNet50 preprocessing.
4. Generate crack segmentation mask using the trained model.
5. Create crack overlay on the original image.
6. Calculate crack percentage.
7. Predict severity level.
8. Display results.

---

## 📊 Severity Classification

| Crack Percentage | Severity |
|-----------------|----------|
| Less than 1% | 🟢 Low |
| 1% – 5% | 🟡 Medium |
| Greater than 5% | 🔴 High |

---

## 🚀 Installation

Clone the repository

```bash
git clone https://github.com/your-username/crack-detection-ai.git
```

Move into the project directory

```bash
cd crack-detection-ai
```

Install dependencies

```bash
pip install -r requirements.txt
```

---

## ▶️ Run the Application

```bash
streamlit run app.py
```

The application will open in your browser.

---

## 📦 Requirements

- Python 3.10+
- TensorFlow
- Streamlit
- OpenCV
- NumPy
- Matplotlib
- Pillow

Install all dependencies using:

```bash
pip install -r requirements.txt
```

---

## 📸 Output

The application displays:

- Original Image
- Predicted Crack Mask
- Crack Overlay
- Crack Percentage
- Severity Level

---

## 📈 Future Improvements

- Multi-class crack classification
- Mobile deployment
- Real-time camera support
- Cloud deployment
- Automatic report generation
- Crack length and width measurement
- Batch image processing

---

## 👨‍💻 Author

**Sambangi Manoj Kumar Naidu**

- B.Tech CSE, SRM University AP
- Machine Learning & Deep Learning Enthusiast

---

## 📄 License

This project is intended for educational and research purposes.
