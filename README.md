# Cry Detection for Smart Baby Cradle 

A machine learning-based cry detection system built using audio signal processing and Support Vector Machine (SVM) classification. This model is designed to be integrated into a Smart Baby Cradle, enabling real-time detection of infant cries and responsive caregiving actions.

---

## Project Overview

The primary goal is to distinguish between **cry** and **non-cry** audio using features extracted from baby sound samples. This system is intended to enhance a smart cradle's capabilities by allowing it to react intelligently to a baby's emotional state.

---

## Features

- Real-time audio classification using trained SVM
- Preprocessed `.wav` files for cry vs. non-cry detection
- MFCC feature extraction from audio samples
- Evaluation via accuracy and confusion matrix
- Ready for integration with IoT/Embedded Systems

---

## Tools & Libraries

- Python 3.10+
- Jupyter Notebook
- Librosa – audio processing
- NumPy, Pandas – data handling
- Scikit-learn – model training
- Matplotlib – visualization

---

## Project Structure


cry-detection-smart-baby-cradle/
│
├── Cry_Detection.ipynb # Jupyter notebook with full implementation
├── dataset/
│ ├── cry/ # Baby crying samples (wav)
│ └── non-cry/ # Other baby sounds (wav)
├── features/
│ └── mfcc_data.csv # Extracted features and labels
├── models/
│ └── svm_model.pkl # Saved trained model
├── README.md # Project description
└── requirements.txt # All necessary dependencies



---

## Output

- **Accuracy:** ~95% on test data
- **Confusion Matrix:** Clear separation between cry and non-cry
- **Significance:** Ensures cradle responds only to real crying, avoiding false triggers

---

## Integration Idea

This model can be deployed on an embedded system like Raspberry Pi or ESP32 with microphone input. When a cry is detected, the cradle can:

- Start gentle rocking
- Alert a parent via mobile notification
- Record logs for monitoring

---

## How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/cry-detection-smart-baby-cradle.git

   cd cry-detection-smart-baby-cradle
   pip install -r requirements.txt
   jupyter notebook Cry_Detection.ipynb


Thanks to the open datasets and Librosa community for making this work possible.



