# 🌾 Crop Disease Predictor

Deep‑learning + Flask app that predicts cotton leaf health from an uploaded image using a trained CNN model.

---

## 📁 Project Structure (as-is)
Crop Disease Predictor/
├── docs/
│   ├── Abstract.pdf
│   ├── Documentation - Crop Disease Predictor.pdf
│   └── Literature Review.pdf
├── flask/
│   ├── app.py
│   ├── model/
│   │   ├── cotton_plant_disease_pred_best_model.h5
│   │   └── v4_cotton_plat_disease_prediction.ipynb
│   ├── static/
│   │   └── (uploads, css/images if any)
│   └── templates/
│       ├── index.html
│       ├── about.html
│       ├── disease_plant.html
│       ├── healthy_plant.html
│       └── healthy_plant_leaf.html
├── model/
│   ├── cotton_plant_disease_pred_best_model.h5   # (duplicate ok — kept as-is)
│   └── v4_cotton_plat_disease_prediction.ipynb
├── presentation/
│   └── presentation.pptx
└── video/
└── Crop_Disease_Demo.mp4

---

> Note: Dataset/test images are hosted externally due to size limits.

---

## 🎥 Demo
The demo video is included:
- `video/Crop_Disease_Demo.mp4`

---

## 🖼️ Dataset & Test Images
Full dataset (train/test images) is on Google Drive:

👉 https://drive.google.com/drive/folders/1mMmooK2LJ8RF5IGTX7F6JF0rJemMnBYu?usp=drive_link

---

## 🧠 Model
The trained CNN model (`cotton_plant_disease_pred_best_model.h5`) is loaded by the Flask app from `flask/model/`:
```python
# in flask/app.py
from tensorflow.keras.models import load_model
model = load_model("model/cotton_plant_disease_pred_best_model.h5")


🚀 Run Locally

Option A — run from project root (recommended)

cd "Crop Disease Predictor"
python3 -m venv .venv
source .venv/bin/activate

pip install -r requirements.txt

# run the Flask app that lives in the flask/ folder
python flask/app.py
# then open http://127.0.0.1:5000

Option B — run from inside the flask folder

If you run from inside flask/, make sure the model path in app.py
is "model/cotton_plant_disease_pred_best_model.h5" (it is).

cd "Crop Disease Predictor"/flask
pip install -r ../requirements.txt
python app.py

🔧 Tech
	•	TensorFlow / Keras, NumPy, Pillow
	•	Flask (Python)
	•	HTML templates + basic static assets

⸻

📚 Docs & Slides

See docs/ for abstract, literature review, and full documentation.
Slides: presentation/presentation.pptx

⸻

👤 Contact

Aditya (Adi) Gujjar — gujjaraditya5555@gmail.com