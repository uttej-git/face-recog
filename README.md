# 📸 Face Recognition Attendance System

A Python-based attendance system that uses face recognition to mark student attendance. It captures faces in real-time using OpenCV and logs attendance **only during defined time slots** (e.g., **morning 9:00–9:30 AM**, **evening till 4:20 PM**). Built with a GUI for easy use in educational institutions like colleges.

---
## ✅ Features

- 🔍 Real-time face detection and recognition using webcam  
- 🧠 Built using `face_recognition`, `OpenCV`, `Tkinter`  
- ⏰ Time-based attendance (e.g., 9–9:30 AM and after 6 hours minimum)  
- 📁 Attendance logged into a `.csv` file  
- 🖼️ Automatically loads known faces from `images/` folder  
- 🖥️ Simple GUI with `Start` button  
- 🛑 Automatically exits after marking or skipping attendance  
- 🔄 Prevents duplicate attendance within the time window  

---
## 📁 Project Structure
```bash
face-attendance/
├── images/             # Folder with known face images
├── attendance.csv      # Log file for storing attendance data
├── main.py             # Backend logic (face recognition + logging)
├── gui_attendance.py   # GUI interface for launching attendance
└── README.md           # Project documentation

```
🛠️ Tech Stack
        Python 3.12+

        OpenCV

        face_recognition

        NumPy, Pandas

        Tkinter (for GUI)

⚙️ How It Works
        Loads known face encodings from the images/ folder

        Opens webcam and detects faces using face_recognition

        Compares captured face with known encodings

        If matched:

        Verifies if the attendance window is valid

        Logs name and timestamp into attendance.csv

        GUI allows launching attendance with a single button click

        Automatically prevents re-entry within the same slot

        🏫 Use Case
        Designed specifically for college classrooms or lab attendance.
        Only allows attendance marking during:

        🕘 Morning Slot: 9:00 AM – 9:30 AM

        🕓 Evening Slot: After a minimum 6-hour gap, up to 4:20 PM

💡 Future Improvements
        Add admin login for attendance control

        Generate PDF reports

        Enable auto email or WhatsApp notifications

        Integrate with a database (MongoDB/PostgreSQL) for persistent storage

👨‍💻 Developed By
Uttej Kumar – B.Tech CSE
(uttej-git)