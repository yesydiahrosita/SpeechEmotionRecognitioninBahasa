# Speech Emotion Recognition in Bahasa
This repository contains a speech dataset in the Indonesian language **with 5 types of emotions**, along with program code for building an emotion classification model using deep learning techniques.  
This project is intended for research and development in the field of Speech Emotion Recognition (SER).

## 📂 Dataset
The dataset includes **1,600 audio samples** in total:  
- **491 positive samples** (250 Happy, 241 Surprise)  
- **619 negative samples** (337 Angry, 282 Sad)  
- **400 neutral samples**
  
You can download the dataset:
- Neutral    [here](https://drive.google.com/drive/folders/1YEDFZEQ1JFbLlt6yWUbXaOcph6Xucxg6?usp=sharing)
- Positive   [here](https://drive.google.com/drive/folders/1CxTeoL75ZcwrK5R2HV4Vd-Uu3r1o5kLS?usp=sharing)
- Negative   [here](https://drive.google.com/drive/folders/1cx36NJ8aHVJY6ZHFDaBSxl6TsxEiGrgK?usp=sharing)
  
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

## 🛡️ Ethical Considerations & Informed Consent

This research involved **actors** as participants for recording emotional speech samples.  
To ensure ethical compliance:  

- **Informed consent** was obtained from all participating actors.  
- The recordings were carried out using prepared scripts corresponding to specific emotion classes (Neutral, Happy, Surprise, Angry, Sad).  
- No personal identifiers (such as names or sensitive information) were included in the dataset.  
- The dataset is intended solely for **research and educational purposes**, and not for commercial use.  

By using actors and scripted speech, this study avoids the use of sensitive real-world lecturer or student data, while still providing a representative and diverse dataset for training and evaluating emotion recognition models.


## 📂 References
If you use this dataset in your research or publications, please cite the related papers listed at the following link: 
1.   
2. Rosita, Y. D., Firmansyah, M. R., & Utami, A. (2025). Exploring bibliometric trends in speech emotion recognition (2020-2024). IAES International Journal of Artificial Intelligence (IJ-AI), 14(4), 3421. https://doi.org/10.11591/ijai.v14.i4.pp3421-3434
 
Proper citation helps acknowledge the original contributors and supports further development of open research in **Speech Emotion Recognition (SER)**.
