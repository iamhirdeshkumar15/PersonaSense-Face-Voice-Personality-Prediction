# PersonaSense: Decoding Personality through Face and Voice

PersonaSense is an AI-powered system that predicts a person's personality traits in real time by analyzing their facial expressions and voice characteristics. Using advanced emotion recognition models, the application maps detected emotions to the Big Five personality traits, offering an innovative perspective on personality analysis.

## 🔍 Project Description

This capstone project aims to develop a multi-modal personality prediction system using facial and vocal emotion analysis. It captures live facial expressions using OpenCV and audio input using a microphone, then processes them using a CNN model (for face emotions) and an SVM model (for audio emotions). Detected emotions are mapped to Big Five personality traits to generate a personality profile.

## 🎯 Objectives

- To capture real-time face and voice data from the user.
- To detect emotional states from facial expressions and vocal cues using machine learning.
- To map emotional states to personality traits (Big Five model).
- To build a web-based interface that interacts with users and presents results.
- To ensure the system works in real-time and is user-friendly.

## 🧠 Technologies Used

- **Python 3.10.7**
- **Flask** – Web framework
- **OpenCV** – Face detection and capture
- **TensorFlow / Keras** – CNN for face emotion detection
- **Sounddevice + Librosa** – Audio capture and processing
- **Scikit-learn** – SVM for voice emotion classification
- **HTML / CSS / JavaScript** – Frontend with optional AI avatar (`<model-viewer>`)
- **Matplotlib / Seaborn** – For visualization (if required)

## 📂 Folder Structure

PersonaSense/
│
├── static/ # CSS, JS, assets
├── templates/ # HTML templates
├── models/ # Trained CNN and SVM models
├── captures/ # Temporary folder for captured images/audio
├── app.py # Main Flask application
├── train_face_emotion_model.py # CNN training for facial emotion detection
├── train_audio_emotion_model.py# SVM training for audio emotion detection
├── requirements.txt # Python dependencies
└── README.md # This file



## ⚙️ Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/PersonaSense-Face-Voice-Personality-Prediction.git
   cd PersonaSense-Face-Voice-Personality-Prediction
   ```

2. **Create a virtual environment**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Train or download models**
   - ***Train face model***
     ```bash
     python train_face_emotion_model.py
     ```
     
   - ***Train audio model***
     ```bash
     python train_audio_emotion_model.py
     ```

5. **Run the application**
   ```bash
   python app.py
   ```

6. **Open in browser**
   ```bash
   http://127.0.0.1:5000/
   ```

## 🧪 How It Works

- Captures images from webcam for 45 seconds (1 frame/sec)
- Records audio in 5-second chunks over 40 seconds
- Analyzes face emotions using a CNN model
- Analyzes voice emotions using an SVM model
- Maps detected emotions to Big Five personality traits:
  - Openness
  - Conscientiousness
  - Extraversion
  - Agreeableness
  - Neuroticism
- Displays a personality report on the web interface


## 🌐 Frontend Features

- 3D AI avatar using <model-viewer>
- Real-time interaction
- User-friendly interface with minimal clicks
- Personality report displayed as a card or chart

## 🧪 Datasets Used

- Facial Emotion Detection: FER 2013
- Voice Emotion Classification: RAVDESS, CREMA-D

## 📈 Personality Mapping Logic

| Emotion      | Associated Traits                |
| ------------ | -------------------------------- |
| Happy        | High Extraversion, Agreeableness |
| Sad          | High Neuroticism                 |
| Angry        | Low Agreeableness                |
| Neutral      | Balanced personality             |
| Surprised    | High Openness                    |
| Disgust/Fear | High Neuroticism, Low Stability  |


## 👨‍💻 Author

- **Name**: Hirdesh Kumar Yadav, Shiva Kumar Chai  
- **College**: Lovely Professional University  
- **Mentor**: Akash Pundir  
- **LinkedIn**: [Add your LinkedIn profile URLs here]  
- **Email**: hirdeshkumaryadav15@gmail.com, shivarajachai@gmail.com

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------


