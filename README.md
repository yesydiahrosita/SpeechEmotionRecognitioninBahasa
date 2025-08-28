# SpeechEmotionRecognitioninBahasa
This repository contains a speech dataset in the Indonesian language **with 5 types of emotions**, along with program code for building an emotion classification model using deep learning techniques.  
This project is intended for research and development in the field of Speech Emotion Recognition (SER).

## 📂 Dataset
The dataset includes **1,600 audio samples** in total:  
- **491 positive samples** (250 Happy, 241 Surprise)  
- **619 negative samples** (337 Angry, 282 Sad)  
- **400 neutral samples**  

The dataset consists of human voice recordings in `.wav` format, categorized into **5 emotion classes**:  
1. Neutral (Netral)  
2. Happy (Bahagia)  
3. Surprise (Terkejut)  
4. Angry (Marah)  
5. Sad (Sedih)  

All recordings are in `.wav` format with an average duration of **3–5 seconds**, which is sufficient to capture emotional characteristics in speech.

The dataset was built from two sources:  
- **Direct recordings** from lecturers with diverse backgrounds and teaching subjects, using wireless microphones for clarity. Each lecturer was provided with speech scripts corresponding to specific emotions.  
- **Publicly available emotional speech recordings** from actors, with proper permission. No personal identifiers are included, so ethical considerations and privacy are preserved.

To minimize bias, the dataset was designed with diversity in speakers and regularly validated during training.

## 📂 Model Scenarios

The classification model was developed through **54 experimental scenarios** designed to evaluate different combinations of methods, architectures, and audio features.  

- **Model Types**: CNN, LSTM, and hybrid CNN-LSTM (3 layers each)  
- **Features Used**: MFCC, Chroma, Mel, Energy, and Zero Crossing Rate (ZCR)  
- **MFCC Variants**: 13, 25, and 40 coefficients to assess their effect on accuracy  
- **Neurons per Layer**: 32, 64, and 128 (varied to balance complexity vs generalization)  

To improve performance and prevent overfitting, **dropout regularization** and **hyperparameter tuning** were applied.  

The use of **MFCC** as the primary feature was chosen due to its effectiveness in representing speech characteristics, especially timbre and tonal variations.  
This systematic approach allows comprehensive comparison across models and helps identify the **optimal configuration** for emotion classification.
