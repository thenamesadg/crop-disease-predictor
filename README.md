# 🌾 Crop Disease Predictor

Deep‑learning + Flask app that predicts cotton leaf health from an uploaded image using a trained CNN model.

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

   Dataset/test images are hosted externally due to size limits.

---

🎥 Demo

Full demo video (hosted on Google Drive):

👉 https://drive.google.com/drive/folders/1D4BoJvP8H84ZlTAvi6V1eoOEpiApKga8?usp=share_link

⸻

🖼️ Dataset & Test Images

Dataset and sample images are also on Drive:

👉 https://drive.google.com/drive/folders/1mMmooK2LJ8RF5IGTX7F6JF0rJemMnBYu?usp=drive_link

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