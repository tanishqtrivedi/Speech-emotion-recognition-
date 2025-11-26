# 🎙️ Speech Emotion Recognition (SER)

A simple project that identifies human emotions from speech audio using
Python, Librosa, and a 1D Convolutional Neural Network (CNN).

## 📌 Overview
This project combines four popular speech-emotion datasets:
- **RAVDESS**
- **CREMA-D**
- **TESS**
- **SAVEE**

The workflow:
1. Load audio file paths and emotion labels  
2. Visualize waveform & spectrogram  
3. Apply audio augmentation (noise, stretch, pitch)  
4. Extract features (ZCR, Chroma, MFCC, RMS, Mel-Spectrogram)  
5. Train a 1D-CNN model  
6. Evaluate using confusion matrix & classification report  

---

## 📁 Project Structure

Speech-Emotion-Recognition/
│── README.md
│── requirements.txt
│── data/ # Place datasets here
│── outputs/
│ ├── data_path.csv
│ ├── features.csv
│ └── models/
│── src/
│ ├── data_utils.py
│ ├── features.py
│ ├── train_model.py
│ └── evaluate.py
└── notebooks/
└── ser_pipeline.ipynb

---

## ⚙️ Installation

```bash
pip install -r requirements.txt
▶️ Running the Project
1. Build dataset index
python src/data_utils.py
2. Extract audio features
python src/features.py
3. Train model
python src/train_model.py
4. Evaluate
python src/evaluate.py
🧠 Model
A simple 1D CNN trained on extracted audio features.
📊 Output
Waveplots
Spectrograms
Training/Validation accuracy
Confusion Matrix
Classification Report
📜 License
MIT
✨ Author
Tanishq Trivedi
