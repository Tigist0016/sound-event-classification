# Sound Event Classification using Machine Learning and Deep Learning Techniques
## Overview
This project focuses on classifying environmental sounds using both classical machine learning and deep learning approaches. The ESC-50 dataset is used, which contains 2000 audio samples across 50 different classes.

## Dataset
- ESC-50 dataset
- 2000 audio samples
- 50 classes (dog bark, rain, cough, etc.)
- Each audio file: 5 seconds
Dataset link:
https://github.com/karolpiczak/ESC-50

## ⚙️ Methods

### Feature Extraction
- MFCC (Mel Frequency Cepstral Coefficients)
- Mel Spectrogram
- 
### Models Implemented
- Machine Learning:
  - KNN
  - SVM (best ML model)
  - Random Forest

- Deep Learning:
  - CNN
  - CRNN (best overall model)

## 🔄 Data Processing
- Audio data converted into MFCC and Mel Spectrogram features
- Normalization applied
- Dataset split:
  - Training: 70%
  - Validation: 15%
  - Test: 15%

## 🔧 Data Augmentation
Applied only to training data:
- Gaussian noise
- Pitch shifting
- Time stretching

## 📈 Results
| Model | Accuracy |
|------ |----------|
| MFCC + SVM | ~63.75% |
| CNN + Mel | ~57.3% |
| CRNN + Mel  | ⭐ ~68.9% |
| CRNN + Mel + Augmentation | ~65.7% |

## 🧠 Best Model
The best performance was achieved using a CRNN model with Mel Spectrogram features reaching approximately **68.3% accuracy**.
