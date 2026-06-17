# Multimodal Voice Phishing Detection System

A multimodal AI system for detecting scam and vishing calls by combining:

✅ Text Analysis (DistilBERT)

✅ Audio Emotion Analysis (MFCC + Random Forest)

✅ Risk Score Fusion

Built using Python, Transformers, Scikit-Learn, PyTorch and HuggingFace.

## Purpose

This repository contains an implementation and evaluation of a multimodal voice-phishing detection methodology inspired by an MDPI research paper.

The objective is to reproduce and analyze the paper's approach as part of a broader research study. Multiple paper implementations are being evaluated independently before selecting or hybridizing methodologies for the final internship project.

## Overview

This project implements a multimodal scam-call detection pipeline inspired by recent MDPI research on voice phishing detection.

The system combines:

- Text-based scam detection using DistilBERT
- TF-IDF + Logistic Regression baseline
- Audio emotion recognition using MFCC features
- Multimodal risk-score fusion

---

## Research Objective

This implementation will be compared against additional voice-phishing detection methodologies. Findings from multiple implementations may later be combined into a unified hybrid architecture.

## Current Status

Implemented Components:

- Text Classification (DistilBERT)
- TF-IDF Baseline
- Audio Feature Extraction (MFCC)
- Audio Classification (Random Forest)
- Multimodal Risk Fusion Prototype

Status: Experimental Implementation

#Architecture

Audio Call
     |
     v
Speech Transcript ----------+
     |                       |
     v                       v
 DistilBERT            MFCC Features
     |                       |
     v                       v
 Scam Score            Emotion Score
           \           /
            \         /
             \       /
              Fusion
                |
                v
          Final Risk

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

## Installation

git clone <repo_url>
cd MDPI_Vishing

pip install -r requirements.txt
jupyter notebook

## Results

<img width="587" height="735" alt="image" src="https://github.com/user-attachments/assets/c3c87733-9c9b-4eb3-8b04-5a94f09fd13f" />
<img width="938" height="363" alt="image" src="https://github.com/user-attachments/assets/a14ed4f3-4a69-40f8-bf13-9bd4b5c01eaf" />
<img width="688" height="336" alt="image" src="https://github.com/user-attachments/assets/d84951a9-3b68-4897-9ac3-a75f9ccf969d" />
<img width="557" height="432" alt="image" src="https://github.com/user-attachments/assets/3656a7c2-3f74-46d0-91f9-45e901aa04f2" />
<img width="717" height="448" alt="image" src="https://github.com/user-attachments/assets/ac068073-77d6-4ae4-943f-71a2f37b3e34" />
<img width="407" height="136" alt="image" src="https://github.com/user-attachments/assets/175dfeb3-a490-4bca-b35f-921ca4a65e69" />

| Model | Accuracy |
|---------|---------|
| TF-IDF + Logistic Regression | 98.8% |
| DistilBERT | 99.2% |
| Audio Random Forest | 92.0% |

## Limitations

- Audio and transcript datasets are independent.
- Fusion uses heuristic weighting.
- This is a reproduction-oriented implementation and not a production-ready system.
- Further comparison with alternative methodologies is ongoing.

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
