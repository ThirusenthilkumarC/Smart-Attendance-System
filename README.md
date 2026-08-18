# 📸 Face Recognition Attendance System

<div align="center">

### 🤖 Smart • Fast • Automated Attendance

A Python-based attendance management system that uses **Face Recognition and Computer Vision** to automatically identify registered students and record their attendance with date and time.

![Python](https://img.shields.io/badge/Python-3.x-blue?style=for-the-badge&logo=python)
![OpenCV](https://img.shields.io/badge/OpenCV-Computer%20Vision-green?style=for-the-badge&logo=opencv)
![SQLite](https://img.shields.io/badge/SQLite-Database-orange?style=for-the-badge&logo=sqlite)
![Status](https://img.shields.io/badge/Status-Under%20Development-yellow?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-red?style=for-the-badge)

</div>

---

## 📌 About The Project

**Face Recognition Attendance System** is a smart attendance management application developed using Python.

Instead of manually taking attendance, the system uses a webcam to detect and recognize registered students. Once a student is recognized, their attendance is automatically recorded along with the current date and time.

This project demonstrates the practical use of:

- 🐍 Python Programming
- 👁️ Computer Vision
- 🤖 Face Recognition
- 🗄️ Database Management
- 📊 Attendance Automation

---

## ✨ Features

### 👤 Student Management

- Register new students
- Store student name and roll number
- Capture student face using webcam
- Maintain student records

### 📷 Face Recognition

- Real-time webcam detection
- Detect faces automatically
- Recognize registered students
- Display recognized student information

### ✅ Automatic Attendance

- Automatically mark attendance
- Record current date
- Record current time
- Prevent duplicate attendance entries
- Store attendance securely

### 📊 Attendance Records

- View attendance history
- Search attendance records
- Filter attendance by date
- Export attendance data

### 🗄️ Database

- SQLite database support
- Student information storage
- Attendance information storage
- Easy local data management

---

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| 🐍 Python | Main Programming Language |
| 👁️ OpenCV | Computer Vision & Webcam |
| 🧠 Face Recognition | Face Identification |
| 🔢 NumPy | Numerical Processing |
| 🗄️ SQLite | Database |
| 📄 CSV | Attendance Export |
| 🖥️ Tkinter / Flask | User Interface |

---

## 🏗️ System Architecture

```text
                 ┌─────────────────────┐
                 │       User          │
                 └──────────┬──────────┘
                            │
                            ▼
                 ┌─────────────────────┐
                 │   Application UI    │
                 └──────────┬──────────┘
                            │
             ┌──────────────┴──────────────┐
             │                             │
             ▼                             ▼
    ┌─────────────────┐          ┌─────────────────┐
    │ Student         │          │ Attendance      │
    │ Registration    │          │ Module          │
    └────────┬────────┘          └────────┬────────┘
             │                            │
             ▼                            ▼
    ┌─────────────────┐          ┌─────────────────┐
    │ Face Capture    │          │ Webcam          │
    └────────┬────────┘          └────────┬────────┘
             │                            │
             ▼                            ▼
    ┌─────────────────┐          ┌─────────────────┐
    │ Face Encoding   │          │ Face Detection  │
    └────────┬────────┘          └────────┬────────┘
             │                            │
             └──────────────┬─────────────┘
                            ▼
                 ┌─────────────────────┐
                 │ Face Recognition    │
                 └──────────┬──────────┘
                            │
                            ▼
                 ┌─────────────────────┐
                 │ Attendance Database │
                 └──────────┬──────────┘
                            │
                            ▼
                 ┌─────────────────────┐
                 │ Reports / History   │
                 └─────────────────────┘
