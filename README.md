# EEG-Based Depression Detection using Deep Learning Models

This project presents a comparative study of three deep learning architectures — LSTM, CNN-LSTM, and Transformer — for classifying Major Depressive Disorder (MDD) using EEG signals. The models are designed to analyze temporal brain activity patterns, perform robust classification, and handle variability and noise in real-world EEG data.

---

## 🧠 Project Overview

- **Objective**: Develop and compare deep learning models for classifying depression using EEG time-series data.
- **Models Implemented**:
  - Long Short-Term Memory (**LSTM**)
  - Convolutional Neural Network + LSTM (**CNN-LSTM**)
  - Transformer with Self-Attention (**Transformer**)
- **Noise Handling**:
  - Variance-based feature filtering
  - Gaussian noise-based perturbation

## 📊 Dataset Description

- **Input Type**: Resting-state EEG signals (64 channels)
- **Subjects**: Control and MDD-labeled individuals
- **Features**: Temporal, statistical, spectral, and entropy-based signals extracted from five brain regions
- **Preprocessing**:
  - Filtering (0.5–70 Hz), 50 Hz notch
  - ICA-based noise removal
  - Segmentation into fixed-length time windows
  - Standard normalization and feature selection

---

## 🚀 Getting Started

### 1. Clone the Repository
git clone https://github.com/yourusername/eeg-depression-detection.git
cd eeg-depression-detection

2. Install Dependencies
Create a virtual environment (optional but recommended), then install packages:
pip install -r requirements.txt

3. Run Notebooks
Open each notebook in Jupyter or Google Colab:
LSTM_MODEL.ipynb
CNN_LSTM_MODEL.ipynb
TRANSFORMER_MODEL.ipynb
Follow the instructions in each notebook to train and evaluate models.

📈 Model Performance Summary
Model	    Accuracy (Clean)	Accuracy (Noisy)
LSTM	          98.6%	         ~98.6%
CNN-LSTM	      89.7%	          85.3%
Transformer	    98.6%	          96.2%

📌 Key Features
Region-specific feature extraction from EEG
Deep autoencoder-generated features for richer representation
Dual feature selection for robustness
5-fold cross-validation for evaluation
Supports clean and perturbed EEG data scenarios

⚙️ Future Enhancements
Add a real-time EEG processing pipeline
Integrate additional physiological signals (HRV, GSR)
Improve cross-subject generalization
Deploy models on edge devices or wearables

📬 Contact
For questions or collaboration inquiries, feel free to contact the repository maintainer.

Let me know if you'd like:
- A `requirements.txt` generated for the code
- A badge section (like Python version, Colab badge, etc.)
- A license section

I'm happy to help you polish it for upload.
