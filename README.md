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
