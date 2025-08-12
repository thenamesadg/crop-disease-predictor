# 🌾 Crop Disease Predictor

A deep learning-powered web application that predicts cotton plant diseases from leaf images using a trained Convolutional Neural Network (CNN), deployed via Flask.

---

## 📌 Project Overview

This project helps farmers and agricultural experts identify common cotton plant diseases early using image classification techniques.  
The model is a CNN trained on a labeled dataset of healthy and diseased cotton leaves.  

Users can upload a cotton leaf image and instantly receive:  
- Disease classification (or healthy result)  
- Recommended treatment suggestions  

---

## 🚀 Features
- 🧠 **Trained CNN model** for cotton leaf disease detection  
- 🌐 **Flask-based web app** for real-time predictions  
- 📤 **Image upload support**  
- 💡 **Remedy suggestions** for detected diseases  
- 🎨 Simple and accessible **UI**  

---

## 📂 Project Structure
```text
Crop Disease Predictor/
├── docs/
│   ├── Abstract.pdf
│   ├── Documentation - Crop Disease Predictor.pdf
│   └── Literature Review.pdf
│
├── flask/
│   ├── app.py
│   ├── model/
│   │   ├── cotton_plant_disease_pred_best_model.h5
│   │   └── v4_cotton_plat_disease_prediction.ipynb
│   ├── static/
│   │   └── user_uploaded/  (runtime uploads)
│   └── templates/
│       ├── index.html
│       ├── about.html
│       ├── disease_plant.html
│       ├── healthy_plant.html
│       └── healthy_plant_leaf.html
│
├── model/
│   ├── cotton_plant_disease_pred_best_model.h5
│   └── v4_cotton_plat_disease_prediction.ipynb
│
├── presentation/
│   └── presentation.pptx
│
└── README.md
```

> **Note:** Large assets like the dataset and demo video are hosted on Google Drive.

---

## 🎥 Demo Video

📹 **[Watch the full demo on Google Drive](https://drive.google.com/drive/folders/1D4BoJvP8H84ZlTAvi6V1eoOEpiApKga8?usp=share_link)**

---

## 🖼️ Dataset & Test Images

📂 **[Download dataset and test images from Google Drive](https://drive.google.com/drive/folders/1mMmooK2LJ8RF5IGTX7F6JF0rJemMnBYu?usp=drive_link)**

---

## 🧠 Tech Stack
- **Python**: TensorFlow, Keras, NumPy, OpenCV, Pillow  
- **Flask** for web deployment  
- **HTML, CSS** (via templates)  

---

## ⚙️ How to Run Locally

1. **Clone the repository**
```bash
git clone https://github.com/thenamesadg/crop-disease-predictor.git
cd "Crop Disease Predictor"
```

2. **Create and activate a virtual environment**
```bash
python3 -m venv .venv
source .venv/bin/activate
```

3. **Install dependencies**
```bash
pip install -r requirements.txt
```

4. **Run the Flask app**
```bash
cd flask
python app.py
```

5. **Open your browser** and visit:
```
http://127.0.0.1:5000
```

---

## 📚 Documentation
- See `/docs` for Abstract, Literature Review, and complete project documentation.  
- `/presentation` contains the project presentation slides.

---

## 🙌 Credits
Developed as part of a university research project.  
**Team:** TEAM_4078  

**Author:** Aditya (Adi) Gujjar  
📧 [gujjaraditya5555@gmail.com](mailto:gujjaraditya5555@gmail.com)
