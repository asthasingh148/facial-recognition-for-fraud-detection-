
# Real-Time Face Recognition with Anti-Spoofing | Fraud Prevention System

This project is a real-time face recognition system with built-in anti-spoofing measures using Convolutional Neural Networks (CNN). It aims to detect and verify human faces through a webcam, generate a dataset, train a deep learning model, and prevent spoofing attacks (like using photos or videos) by checking for live human presence (blink, head movement, etc.).


#  Key Features

- Real-time webcam-based face capture
- Human detection using YOLO (via Ultralytics)
- Automatic dataset generation
- Face recognition using CNN (Keras + TensorFlow)
- Anti-spoofing through liveness detection (blink/head move)
- Speech-to-text and text-to-speech capabilities
- Local logging of recognition events


#  Technology Stack

| Library/Tool           | Purpose                                       |
|------------------------|-----------------------------------------------|
| `OpenCV (cv2)`         | Webcam access and image processing            |
| `Ultralytics YOLO`     | Real-time object/human detection              |
| `TensorFlow / Keras`   | CNN model creation and training               |
| `NumPy`                | Numerical operations                          |
| `sklearn.preprocessing`| Label encoding                                |
| `sklearn.model_selection`| Train-test split                            |
| `pyttsx3`              | Text-to-speech output                         |
| `os`, `time`           | File system and timing tasks                  |



#  How It Works

1. Camera Activation → Starts webcam and checks for human presence.
2. Face Detection → YOLO detects if a human is in the frame.
3. Dataset Creation → Captures multiple face images to create a dataset.
4. Model Training → Trains a CNN using Keras on the collected dataset.
5. Liveness Detection → Validates if the user is real (not a spoof).
6. Face Verification → Matches face using trained model.
7. Text-to-Speech Feedback → Notifies user of success/failure.
8. Logging → Saves authentication logs and timestamps locally.



# Use Cases

- Secure authentication for banking and fintech apps
- Fraud prevention in e-KYC and digital identity verification
- Smart attendance systems
- Automated access control in high-security areas



#  Installation & Setup

# Prerequisites

- Python 3.7 or higher
- Webcam-enabled device
- Recommended: GPU for faster training

# Installation


git clone https://github.com/asthasingh148/face-recognition-anti-spoofing.git
cd face-recognition-anti-spoofing
pip install -r requirements.txt

# Running the Project


# Step 1: Run the main file
python main.py

# Step 2: Train the model after data collection
python train_model.py



# Project Structure


├── dataset/                 # Captured face images
├── model/                   # Saved CNN model
├── logs/                    # Access & verification logs
├── main.py                  # Main application logic
├── train_model.py           # CNN training script
├── requirements.txt         # Python dependencies
└── README.md                # Project overview




# Future Scope

*  Mobile application integration
*  Cloud-based monitoring dashboard
*  Deepfake detection add-on
*  Multi-factor biometric authentication


# Contributors

 astha – (https://github.com/asthasingh148)



