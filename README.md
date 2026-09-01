# Multi-Representation-Feature-Fusion-for-Speech-Based-Parkinson's Disease-Classification-
Deep learning-based voice disease detection using Mel Spectrogram, Gammatone, CQT using MobileNetV3.
# Parkinson's Disease Detection from Voice Signals

## 📌 Project Overview

This project develops a deep learning-based system for detecting Parkinson's Disease (PD) from voice recordings.

The system extracts multiple time-frequency representations from voice signals and uses a
MobileNetV3-Small based architecture with specialized feature processing and fusion modules
for binary classification of Parkinson's Disease and healthy controls.

---

## 🎯 Objective

The main objective is to develop an automated voice-based approach for distinguishing:

- Parkinson's Disease (PD)
- Elderly Healthy Controls (HC)

from speech/audio recordings.

---

## 📊 Dataset

The project uses the **Italian Parkinson's Disease Dataset**.

### Classes Used

- **28 People with PD**
- **22 Elderly Healthy Control**

The Young Healthy Control group is not included in the experiment.

The dataset contains WAV audio recordings from multiple subjects.

> The dataset is not included in this repository. Please obtain the dataset separately
> and configure the dataset path before running the project.

---

## 🔄 Project Workflow

```text
Voice Recordings
       ↓
Audio Preprocessing
       ↓
Mel Spectrogram
       ↓
CQT
       ↓
Gammatone Spectrogram
       ↓
Feature Normalization & Resizing
       ↓
CSRLM
       ↓
FIEM
       ↓
ASFM
       ↓
MobileNetV3-Small
       ↓
Classification
       ↓
Performance Evaluation 
