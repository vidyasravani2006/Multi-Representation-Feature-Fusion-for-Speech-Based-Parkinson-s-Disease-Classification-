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

## ▶️ How to Run

### 1. Clone the Repository

```bash
git clone https://github.com/vidyasravani2006/Voice-Based-Disease-Detection.git
cd Voice-Based-Disease-Detection
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Download the Dataset

- Download the Italian Parkinson's Disease Dataset.
- The project uses the Italian Parkinson's Disease Dataset hosted on Kaggle.
- Add the dataset to your Kaggle Notebook before running the project.
- The notebook uses the following Kaggle dataset path:

Example:

```python
DATASET_PATH = "/kaggle/input/datasets/vidyasravanich/"
        "italian-pd-dataset/italian PD dataset"
```

### 4. Open the Notebook

```bash
Open the project notebook in Kaggle.
Click Add Input.
Search for and add the Italian Parkinson's Disease Dataset.
Verify that the dataset path matches:
DATASET_PATH = "/kaggle/input/datasets/vidyasravanich/italian-pd-dataset/italian PD dataset"
Select GPU in the Kaggle Notebook settings.
Run the notebook cells sequentially from top to bottom.
```

### 5. Run the Project

Run the notebook cells sequentially:

1. Load and preprocess audio files.
2. Extract Mel Spectrogram, Gammatone, and CQT features.
3. Apply CSRLM, FIEM, and ASFM modules.
4. Train the MobileNetV3-Small model with online augmentation.
5. Evaluate the model using Accuracy, Precision, Recall, F1-Score, and ROC-AUC.

### 6. View Results

The notebook generates:

- Classification Metrics
- Confusion Matrix
- Model Performance Results
