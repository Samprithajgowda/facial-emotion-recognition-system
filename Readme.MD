# 🧠 Real-Time Facial Emotion Recognition System

Real-time full-stack facial emotion recognition web application using FastAPI, TensorFlow, and ReactJS.

![Python](https://img.shields.io/badge/Python-3.10-blue)
![FastAPI](https://img.shields.io/badge/FastAPI-Backend-green)
![React](https://img.shields.io/badge/React-Frontend-61DAFB)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.8-orange)
![WebSocket](https://img.shields.io/badge/WebSocket-RealTime-purple)

---

## 🚀 Overview  

This project implements a real-time facial emotion recognition system using a deep learning model integrated into a full-stack web application.

The system captures live video frames from a webcam, transmits them to a FastAPI backend via WebSocket, performs emotion classification using a pre-trained CNN model (FER), and returns predictions to the frontend for real-time display.

---

## 🏗 System Architecture  

```
Phone Camera (Iriun)
        ↓
React Frontend (Video Capture)
        ↓ (WebSocket)
FastAPI Backend
        ↓
TensorFlow FER Model
        ↓
Emotion Prediction (JSON)
        ↓
Frontend Real-Time Display
```

---

## 🎯 Features  

- 🔴 Real-time facial emotion detection  
- 🔁 WebSocket-based communication  
- 🧠 Pre-trained FER deep learning model  
- 📷 OpenCV image processing  
- ⚡ FastAPI backend for low-latency inference  
- 🌐 React frontend with live updates  
- 📱 Phone-to-PC webcam integration using Iriun  

---

## 🛠 Tech Stack  

### Backend  
- FastAPI  
- TensorFlow 2.8  
- FER (Facial Emotion Recognition library)  
- OpenCV  
- NumPy  
- Uvicorn  

### Frontend  
- ReactJS  
- JavaScript  
- WebSocket API  
- HTML / CSS  

---

## ⚙️ Installation & Setup  

### 1️⃣ Clone the Repository  

```bash
git clone https://github.com/your-username/facial-emotion-recognition.git
cd facial-emotion-recognition
```

---

### 2️⃣ Backend Setup  

```bash
cd server
python -m venv venv
.\venv\Scripts\Activate
pip install -r requirements.txt
uvicorn main:app --reload
```

Backend runs at:

```
http://127.0.0.1:8000
```

---

### 3️⃣ Frontend Setup  

Open a new terminal:

```bash
cd emotion-recognition
npm install
npm start
```

Frontend runs at:

```
http://localhost:3000
```

---

## 📷 Webcam Configuration  

This project uses **Iriun Webcam** to connect a mobile phone camera as a virtual webcam for real-time emotion detection.

Steps:
1. Install Iriun Webcam on PC.
2. Install Iriun mobile app.
3. Connect both devices to the same network.
4. Allow browser camera permissions.

---

## 🧩 Technical Challenges Solved  

- Resolved TensorFlow compatibility issues (Python 3.12 → Python 3.10 downgrade).  
- Configured isolated Python virtual environment for backend.  
- Managed Node.js and React dependency setup.  
- Implemented real-time WebSocket communication pipeline.  
- Integrated phone camera as virtual webcam.  

---

## 📊 Emotion Output  

The model predicts emotions such as:

- Happy  
- Sad  
- Angry  
- Fear  
- Surprise  
- Disgust  
- Neutral  

The dominant emotion is selected using maximum probability from the prediction dictionary.

---

## 🚀 Future Improvements  

- Add face-detection validation (handle no-face cases)  
- Display confidence percentage bars  
- Add emotion history graph  
- Convert to image-upload based API  
- Dockerize the backend  
- Deploy to cloud platform  

---

## 📌 Project Motivation  

This project demonstrates full-stack machine learning integration, real-time inference pipelines, and practical environment configuration for deploying deep learning models in web applications.

---
## 📸 Demo


### 🔴 Live Emotion Detection

![Live Detection](assets/live_detection1.png)

### 🏗 System Architecture

![Architecture](assets/architecture.png)

### ⚙ Backend API

![Backend API](assets/live_detection2.png)

## 👩‍💻 Author  

Sampritha J Gowda 


