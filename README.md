# 📞 EchoGuard: Multimodal Voice Phishing Detection System

A multimodal AI system for detecting scam and vishing calls by combining:

✅ Text Analysis (DistilBERT)

✅ Audio Emotion Analysis (MFCC + Random Forest)

✅ Risk Score Fusion

Built using Python, Transformers, Scikit-Learn, PyTorch and HuggingFace.
## Overview

This project implements a multimodal scam-call detection pipeline inspired by recent MDPI research on voice phishing detection.

The system combines:

- Text-based scam detection using DistilBERT
- TF-IDF + Logistic Regression baseline
- Audio emotion recognition using MFCC features
- Multimodal risk-score fusion

---

## Datasets

### Text Dataset
Composite Scam Transcript Dataset

### Audio Dataset
RAVDESS Emotional Speech Dataset

---

## Implemented Models

### Text Branch
- TF-IDF + Logistic Regression
- DistilBERT Fine-Tuning

### Audio Branch
- MFCC Feature Extraction
- Random Forest Classifier

### Fusion
Final Risk Score =
0.7 × Text Score +
0.3 × Audio Score

---

## Results

| Model | Accuracy |
|---------|---------|
| TF-IDF + Logistic Regression | 98.8% |
| DistilBERT | 99.2% |
| Audio Random Forest | 92.0% |

---

## Future Work

- Real-time scam call monitoring
- End-to-end multimodal transformers
- Aligned scam-call audio datasets
- Explainable risk scoring

---

## Author

Thrupthi G D

PES University
CSE (AIML)
