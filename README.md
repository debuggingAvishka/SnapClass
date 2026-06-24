# SNAPCLASS 🎓

An AI-powered smart attendance management system that uses **Face Recognition** and **Voice Recognition** to automate classroom attendance.

🌐 **Live Demo:** https://snapclass-am.streamlit.app/

---

## Overview

SNAPCLASS is designed to simplify attendance tracking in educational institutions by leveraging Artificial Intelligence.

Teachers can create subjects, enroll students, upload classroom photos, and automatically mark attendance using facial recognition. Students can register using Face ID and optionally enroll their voice for voice-based attendance.

The project combines modern web technologies with machine learning to provide a seamless and secure attendance experience.

---

## Features

### 👨‍🏫 Teacher Features

* Teacher registration and login
* Create and manage subjects
* Generate subject enrollment codes
* Share subject codes with students
* Upload classroom photos
* AI-powered attendance processing
* View attendance records
* Manage enrolled students

### 👩‍🎓 Student Features

* Face ID login
* New student registration
* Voice enrollment (optional)
* Subject enrollment using unique codes
* View enrolled subjects
* View attendance statistics
* Unenroll from subjects

### 🤖 AI Features

* Face Detection
* Face Embedding Generation
* Face Recognition-based Attendance
* Voice Embedding Generation
* Voice-based Attendance Support
* Automated Attendance Prediction

---

## Tech Stack

### Frontend

* Streamlit

### Backend

* Python

### Database

* Supabase

### Machine Learning

* Face Recognition
* Resemblyzer
* NumPy
* Pillow (PIL)

### Authentication

* Face-Based Authentication
* Voice-Based Verification
* BCrypt Password Hashing

---

## Project Structure

```text
SNAPCLASS/
│
├── app.py
├── src/
│
├── screens/
│   ├── teacher_screen.py
│   ├── student_screen.py
│
├── components/
│   ├── dialog_add_photo.py
│   ├── dialog_create_subject.py
│   ├── dialog_enroll.py
│   └── ...
│
├── database/
│   ├── config.py
│   └── db.py
│
├── pipelines/
│   ├── face_pipeline.py
│   └── voice_pipeline.py
│
└── ui/
    └── base_layout.py
```

---

## Installation

### Clone Repository

```bash
git clone https://github.com/YOUR_USERNAME/SNAPCLASS.git
cd SNAPCLASS
```

### Create Virtual Environment

```bash
python -m venv venv
```

### Activate Environment

#### Windows

```bash
.\venv\Scripts\Activate.ps1
```

#### Linux / macOS

```bash
source venv/bin/activate
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Configure Environment Variables

Create a `.env` file:

```env
SUPABASE_URL=your_supabase_url
SUPABASE_KEY=your_supabase_key
```

### Run Application

```bash
streamlit run app.py
```

---

## How It Works

### Student Registration

1. Student captures facial image.
2. Face embeddings are generated.
3. Optional voice enrollment is performed.
4. Data is stored in Supabase.

### Student Login

1. Student captures a live image.
2. Face embeddings are extracted.
3. AI matches embeddings with registered students.
4. Student is authenticated automatically.

### Attendance Process

1. Teacher uploads classroom photos.
2. Faces are detected.
3. Face embeddings are generated.
4. AI compares detected faces with enrolled student embeddings.
5. Attendance records are created automatically.

---

## Future Improvements

* Real-time attendance tracking
* Attendance analytics dashboard
* CSV and Excel exports
* Multi-class attendance support
* Mobile application
* Voice-only attendance mode
* Attendance reports with charts

---

## Live Application

https://snapclass-am.streamlit.app/

---

## Author

**Avishka Mittal**

Computer Science & Engineering Student
Jabalpur Engineering College

GitHub: https://github.com/debuggingavishka

---

## License

This project is intended for educational and learning purposes.
