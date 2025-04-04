# Audio Deepfake Detection

## 📌 Overview
This repository contains the implementation of an **Audio Deepfake Detection** model using **XGBoost Classifier** on extracted audio features. The project aims to detect AI-generated human speech by leveraging spectral and temporal audio characteristics.

## Workflow (Simplified in 5 Steps)

1️⃣ **Convert FLAC to WAV**  
   - The dataset is in **FLAC format**, so we first **convert it to WAV** for easier processing.  

2️⃣ **Preprocess the Audio**  
   - Extract important features like **, spectrograms** to understand the sound patterns.  

3️⃣ **Train the Machine Learning Model**  
   - Use models like **Transformers,  XGBoost** to learn differences between **real and fake audio.**  

4️⃣ **Evaluate the Model**  
   - Test the trained model with new audio files and measure accuracy using **confusion matrix, precision, and recall.**  

5️⃣ **Predict and Detect Deepfakes**  
   - The model analyzes a new audio file and predicts whether it is **real or AI-generated (fake).**  



## 📂 Dataset Acquisition
The dataset used in this project is **DEEP-VOICE**, which consists of AI-generated and real human speech samples. Additional datasets were referenced from:
- [ASVspoof 5](https://zenodo.org/records/14498691)
- flac_D of 6.6gb



## 🚀 Project Structure
```
Audio_Deepfake_Detection/
│── data/                        # Dataset storage
│   ├── flac_D/                  # Raw FLAC files
│   ├── wav_D_random10k/         # Converted WAV files
│   ├── features.csv             # Extracted audio features (from Excel file)
│   ├── mel_spectrograms.npy      # Precomputed spectrograms
│   
│
├── xgboost_deepfake_detector.pkl  # Trained XGBoost model
│
├── Audio Deepfake Detection Take.ipynb  # Main notebook for research & implementation
│
│── requirements.txt              # Dependencies list
```



## Setup Instructions

### 1. Clone the Repository
First, download the project from GitHub:
```bash
git clone https://github.com/A-A-D-I-C-O-D-E/Audio-Deepfake-Detection.git
cd Audio-Deepfake-Detection
```

### 2. Create a Virtual Environment (Recommended)
To avoid conflicts, create and activate a virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On macOS/Linux
venv\Scripts\activate  # On Windows
```

### 3. Install Required Dependencies
Make sure you have all necessary libraries installed:
```bash
pip install -r requirements.txt
```

### 4. Run the Jupyter Notebook
Start Jupyter Notebook to train and test the deepfake detection model:
```bash
jupyter notebook
```
Then, open the notebook file and follow the steps inside.


## 📝 References
- [Audio Deepfake Detection Papers](https://github.com/media-sec-lab/Audio-Deepfake-Detection)
- [Librosa Documentation](https://librosa.org/doc/main/index.html)
- [XGBoost Documentation](https://xgboost.readthedocs.io/)


