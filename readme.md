# 🧠 Low-Cost Smart Board – SIH 2023 Final Project

A **self-contained, AI-powered Smart Classroom Assistant** designed by **Team Tech Trojans** for the Smart India Hackathon 2023 finals. Built on **Raspberry Pi**, this hardware-integrated solution combines **voice intelligence**, **gesture control**, and **digital note-taking**, all under ₹20,000.

No external USB cables, laptops, or systems required — just plug in, power up, and go smart.

---

## 🎯 Project Highlights

* 🔌 **Fully embedded** system using **Raspberry Pi**
* 🎤 Real-time **voice monitoring** with speech-to-text & decibel alerts
* ✋ **Gesture-based slide control** (no touch needed!)
* 📝 Smart note-taking, QR sharing, and TTS reading
* 📦 Standalone design – **no USB cables**, **no laptops**, **no cloud dependency**
* 💰 **Total hardware + software cost < ₹20,000**
* 🛠️ Elegant and portable **hardware casing**

---

## ✨ Features

### 🎤 Voice Intelligence

* Real-time **Speech-to-Text** transcription using `speech_recognition`
* **Decibel Monitoring** with auto-alerts to HOD/tutor via email
* React-based UI for **live transcription and noise level visualization**

### ✋ Gesture-Based Slide Control

* Hand tracking using **OpenCV** + **cvzone**
* Turn slides forward/backward with simple hand gestures
* Teacher never needs to touch the system

### 📅 Smart Class Scheduler

* **Auto hourly bell alerts**
* End-of-class detection with **popup + TTS reminders**
* Time schedule driven by **custom config**

### 📚 Text-to-Speech Assistant

* Converts any note into **natural-sounding speech**
* Uses `pyttsx3` and React interface for instant voice playback

### 📝 Smart Notes

* Create, edit, and save notes with a **rich text React editor**
* Save/load locally with `.txt` file support
* Perfect for class notes and instructions

### 📦 QR Code Generator

* Share PPTs or Google Drive links via QR codes
* Generated with `segno` and styled with colors
* Students can scan and instantly access material

### ✅ Attendance System

* Extendable `attendance.py` module using webcam for face-based logging

---

## 🛠️ Hardware Stack

| Component           | Description                 |
| ------------------- | --------------------------- |
| 💻 Raspberry Pi 4   | Primary compute unit        |
| 📷 USB Camera       | For gesture & voice capture |
| 🔊 Speaker          | For voice alerts & TTS      |
| 🖥️ HDMI Display    | Smart board display         |
| 🪛 Custom Enclosure | Sleek portable casing       |
| ⚡ Power Supply      | No laptop or USB needed     |

---

## 💻 Software Stack

| Layer        | Technology                                   |
| ------------ | -------------------------------------------- |
| UI/UX        | React.js, Material UI, CSS                   |
| Backend API  | Python Flask                                 |
| AI/ML        | OpenCV, speech\_recognition, pyttsx3, cvzone |
| QR & Notes   | segno, tkinter                               |
| Alert System | Brevo SMTP, email, text-to-speech            |

---

## 🚀 Setup & Installation

### 🧠 Backend (Flask + Python)

```bash
cd backend/
pip install -r requirements.txt
python app.py
```

### 🖼️ Frontend (React UI)

```bash
cd frontend/
npm install
npm start
```

### Optional `.env` for Email Alerts

```env
EMAIL_USERNAME=lipekadhamodharan@gmail.com
EMAIL_PASSWORD=your_brevo_smtp_key
FLASK_SERVER_URL=http://127.0.0.1:5000
```

---

## 💰 Cost Breakdown

| Item                   | Approx. Cost (₹) |
| ---------------------- | ---------------- |
| Raspberry Pi 4B        | ₹7,000           |
| USB Camera & Mic       | ₹1,000           |
| Speaker & Display      | ₹3,000           |
| Acrylic Enclosure      | ₹1,000           |
| Electronics (misc.)    | ₹1,000           |
| Development & Software | ₹7,000 (DIY)     |
| **Total**              | **< ₹20,000**    |

---

## 📊 Success Metrics

| Metric                 | Value                   |
| ---------------------- | ----------------------- |
| STT Accuracy           | \~91% (classroom noise) |
| Gesture Response Delay | < 0.4 sec               |
| Email Alert Latency    | < 2 sec                 |
| QR Code Generation     | \~1 sec                 |
| TTS Response           | Instant                 |

---

## 🏆 Submission Details

| Category  | Description                |
| --------- | -------------------------- |
| Hackathon | Smart India Hackathon 2023 |
| Track     | Hardware Edition – Finals  |
| PS ID & Ministry  | SIH1430 / Ministry of Education, India  |
| Team      | **Tech Trojans**           |
| College   | SKCET, Coimbatore          |

---

## 💡 Future Enhancements

* Add **offline face-based attendance tracking**
* Integrate with **school ERP systems**
* Add **dashboard analytics** for HODs
* Build **mobile companion app**
