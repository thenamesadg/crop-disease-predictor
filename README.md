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

## 📁 Project Structure

```text
Crop Disease Predictor/
├─ docs/
│  ├─ Abstract.pdf
│  ├─ Documentation - Crop Disease Predictor.pdf
│  └─ Literature Review.pdf
├─ flask/
│  ├─ app.py
│  ├─ model/
│  │  ├─ cotton_plant_disease_pred_best_model.h5
│  │  └─ v4_cotton_plat_disease_prediction.ipynb
│  ├─ static/
│  │  └─ user_uploaded/        (runtime uploads)
│  └─ templates/
│     ├─ index.html
│     ├─ about.html
│     ├─ disease_plant.html
│     ├─ healthy_plant.html
│     └─ healthy_plant_leaf.html
├─ model/
│  ├─ cotton_plant_disease_pred_best_model.h5   (duplicate kept as-is)
│  └─ v4_cotton_plat_disease_prediction.ipynb
├─ presentation/
│  └─ presentation.pptx
└─ video/
   └─ (video hosted externally – see link below)

   > **Note:** Large assets like the dataset and demo video are hosted on Google Drive.

---

## 🎥 Demo Video

📹 **[Watch the full demo on Google Drive](https://drive.google.com/drive/folders/1D4BoJvP8H84ZlTAvi6V1eoOEpiApKga8?usp=share_link)**

---

## 🖼️ Dataset & Test Images

📂 **[Download dataset and test images from Google Drive](https://drive.google.com/drive/folders/1mMmooK2LJ8RF5IGTX7F6JF0rJemMnBYu?usp=drive_link)**

⸻

🧠 Model

The Flask app loads the model from flask/model/:
from tensorflow.keras.models import load_model
model = load_model("model/cotton_plant_disease_pred_best_model.h5")

---

🚀 Run Locally

Option A — run from project root (recommended)
cd "Crop Disease Predictor"
python3 -m venv .venv
source .venv/bin/activate

pip install -r requirements.txt

python flask/app.py
# then open http://127.0.0.1:5000

Option B — run from inside the flask folder
cd "Crop Disease Predictor"/flask
pip install -r ../requirements.txt
python app.py

---

🔧 Tech
	•	TensorFlow / Keras, NumPy, Pillow
	•	Flask (Python)
	•	HTML templates + basic static assets

⸻

📚 Docs & Slides
	•	See docs/ for abstract, literature review, and full documentation
	•	Slides: presentation/presentation.pptx

⸻

👤 Contact

Aditya (Adi) Gujjar — gujjaraditya5555@gmail.com