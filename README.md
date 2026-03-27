# ⏰ AI Alarm Clock with Face Recognition

An intelligent alarm clock system that ensures users wake up on time by requiring **face verification** to stop the alarm.
Built using modern computer vision and web technologies, this project improves wake-up reliability through biometric authentication.

---

## 🚀 Features

### 🔐 Face Registration

- Captures multiple face samples using webcam
- Generates a stable **128-dimensional face encoding**
- Stores user data locally for privacy

### ⏰ Smart Alarm Scheduling

- Supports **12-hour (AM/PM) format**
- Alarm settings persist using local storage
- Easy-to-use interface for setting alarms

### 🧠 Face Verification System

- Alarm stops only after successful face recognition
- Uses **multi-frame verification** for better accuracy
- Real-time detection using webcam

### 🔊 Alarm Mechanism

- Continuous alarm sound using `pygame`
- Stops automatically after successful verification

---

## 📂 Data Handling

No external dataset is used. All data is generated locally.

- Face Encoding → `data/user_face_encoding.pkl`
- Alarm Data → `data/alarm_state.json`

🔒 **Privacy Note:** All user data remains on the local machine.

---

## 🤖 Model & Working

- Uses `face_recognition` library (based on **dlib**)
- Generates **128-D facial embeddings**
- Face matching done using **Euclidean Distance**
- Match condition: distance < 0.5

---

## 🛠️ Technologies Used

| Component        | Technology              |
| ---------------- | ----------------------- |
| Web Interface    | Streamlit               |
| Face Recognition | face_recognition (dlib) |
| Image Processing | OpenCV                  |
| Alarm Sound      | pygame                  |
| Data Storage     | JSON, Pickle            |
| Others           | NumPy, datetime         |

---

## ▶️ How to Run the Project

1. Clone the repository
2. Install required libraries:

   ```bash
   pip install -r requirements.txt
   ```

3. Run the application:

   ```bash
   streamlit run app.py
   ```

---

## 📌 Future Enhancements

- Mobile app integration
- Cloud-based face storage
- Multiple user support
- Improved AI accuracy

---

## ⭐ Project Highlights

- Combines **AI + IoT + Computer Vision**
- Real-world problem solving (oversleeping)
- Fully local and privacy-focused system
