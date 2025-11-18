🛡️ *Self-Defense Pose Recognition System*

A real-time pose detection system built using computer vision and machine learning techniques to detect self-defense stances. This project helps identify whether a user is performing specific self-defense positions using a webcam input or uploaded video stream.


🚀 Overview

This project uses OpenCV, MediaPipe, and Machine Learning to classify human body poses related to basic self-defense postures. By analyzing key body landmarks, the model predicts which defensive stance the user is performing.

The system can be used for:

Self-defense training

Fitness monitoring

Real-time posture correction

Educational demonstrations


✨ Features

🎥 Real-time pose detection using webcam

🧍 Human landmark tracking using MediaPipe

🤖 ML-based classification of self-defense poses

📊 Pose accuracy detection

💻 Lightweight & runs on CPU

📦 Easy to set up and extend


🏗️ Tech Stack

Frontend / Interface

Python OpenCV GUI window

Real-time video capture

Backend

OpenCV

MediaPipe

NumPy

scikit-learn / TensorFlow Lite (depending on model choice)

ML

Pose landmark extraction

Feature engineering (angles, distances)

Multi-class classifier for poses


🔍 Poses Detected

You can customize this list depending on your implementation:

Guard Stance

Blocking Pose

Defensive Lean

Arm Raise Defense

Kick-ready Defense

Attack-ready Posture


📂 Project Structure

Self-Defense-Pose-Recognition-System/
│── dataset/                    # Training images or CSV landmark data
│── models/                     # Trained ML model files
│── utils/                      # Helper scripts
│── pose_module.py              # Landmark extraction logic
│── train_model.py              # Script to train the classifier
│── test_realtime.py            # Real-time prediction script
│── README.md                   # Documentation
│── requirements.txt            # Dependencies


🔧 Installation & Setup
1. Clone the repository
git clone https://github.com/<your-username>/Self-Defense-Pose-Recognition-System.git
cd Self-Defense-Pose-Recognition-System

2. Install dependencies
pip install -r requirements.txt

3. Run real-time detection
python test_realtime.py


🧠 How It Works
Step 1 — Landmark Extraction

MediaPipe Pose extracts 33 key landmarks from the human body.

Step 2 — Feature Engineering

Angles and distances between body joints are calculated to represent the posture numerically.

Step 3 — Pose Classification

The extracted features are passed to a trained ML model, such as:

Random Forest

SVM

KNN

TensorFlow neural network

Step 4 — Real-Time Display

The system overlays:

Detected pose

Confidence score

Pose landmarks

Onto the user’s webcam feed.


📈 Training Your Own Model

You can add more poses or improve accuracy by training again:

python train_model.py

Place your labeled pose data in the dataset/ folder before training.


🧪 Example Output

You can add images here:

📷 Example:
- Webcam preview with pose keypoints
- Predicted label: "Guard Stance: 92% accuracy"


📜 License

This project is licensed under the MIT License.


👤 Author

Aadhya Nigam [(https://github.com/AadhyaNigam)]
