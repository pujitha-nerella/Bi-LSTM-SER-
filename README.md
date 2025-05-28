## Project Overview
This project focuses on **Speech Emotion Recognition (SER)** using a hybrid deep learning architecture combining **BiLSTM** and **self-attention**. The goal is to classify emotions from speech by leveraging powerful **pretrained transformer-based models** for feature extraction.
## Models Used for Feature Extraction

* **WavLM-Large**
* **HuBERT-XLarge**
* **Whisper-Large**
* **wav2vec 2.0 Large**
* **XLSR-53**
* **Data2Vec Audio-Large**

## Data Preprocessing
To ensure high-quality inputs, the following steps were applied:
* **Wiener Filtering** – Reduces background noise
* **Normalization** – Maintains consistent amplitude
* **Voice Activity Detection (VAD)** – Removes silences
* **Resampling** – Standardizes audio sampling rates
## Data Augmentation

* **Time Shift**
* **Pitch Shift**
* **Gaussian Noise Addition**
* **Time Stretch**
* **Gain Adjustment**

## Model Architecture
* **BiLSTM**: Captures forward and backward temporal dependencies.
* **Self-Attention Mechanism**: Focuses on emotionally salient segments in the speech.
* **Fully Connected Layers**: Classify into one of the emotion categories (e.g., Happy, Sad, Angry, etc.).
## Datasets Used
1. **RAVDESS** – 8 emotions (augmented to \~6000 samples)
2. **SAVEE** – 7 emotions (augmented to \~2000 samples)
3. **TESS** – 7 emotions (augmented to \~6000 samples)
## Evaluation Metrics
* **Accuracy (Weighted & Unweighted)**
* **Precision, Recall, F1-Score**
* **Inference Time**
* **Model Size**
