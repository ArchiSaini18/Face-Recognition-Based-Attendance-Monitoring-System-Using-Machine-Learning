🎯 Face Recognition–Based Attendance Monitoring System

This project implements an automated attendance system using computer vision and a graphical user interface (GUI) built with Tkinter. 
The system detects and recognizes faces of registered users via webcam, logs their attendance in real time, and even allows sending daily attendance reports via email.

📌 Project Overview

In this project, we:

• Capture student images via webcam and store them in a dataset.
• Train a face recognition model (LBPH algorithm) using OpenCV.
• Match faces in real time and automatically mark attendance.
• Build a GUI for managing registration, password security, and email notifications.
• Provide options to view, delete, or send attendance records.

📂 Dataset

• Created Locally via webcam (TrainingImage folder).
• Stored Data: Student ID, Name, and captured face images.
• Attendance Files: CSV files saved daily (e.g., Attendance_31-10-2025.csv).
• Details File: StudentDetails.csv containing registration info.

🛠️ Technologies Used

• Python 3.x
• Tkinter – GUI development
• OpenCV – face detection & recognition
• NumPy, Pandas – data handling
• CSV module – attendance record keeping
• smtplib – for sending attendance reports via email
• PIL (Pillow) – for handling images

🤖 Model Logic

Face Detection: Uses the Haar Cascade classifier (haarcascade_frontalface_default.xml) to detect faces from webcam feed.

Feature Extraction: Converts face regions to grayscale images.

Training: Uses LBPH (Local Binary Pattern Histogram) algorithm to train a face recognizer model.

Recognition: Matches real-time faces against trained profiles.

Attendance Logging: When a face is recognized, logs (ID, Name, Date, Time) into a CSV file.

🧭 Workflow

Student Registration → Capture Images → Train Face Recognizer →
Face Detection in Real Time → Identify → Mark Attendance →
Export/Send Attendance

💼 GUI Features
Feature	Description
• Take Images	Capture 100+ face samples for a new student.
• Save Profile	Trains the recognizer after password verification.
• Take Attendance	Recognizes faces and logs attendance in a CSV.
• Change Password	Secure admin access for training new faces.
• Send Attendance Email	Automatically sends attendance CSV via email.
• Delete Data	Options to remove old CSVs or training images.
• Contact Us	Displays developer contact information.

📊 Visualization & Data Handling
• Attendance displayed in GUI as a table (TreeView) with columns: ID, Name, Date, Time.
• Clock and date shown live on the interface.
• Attendance CSVs can be automatically emailed or deleted via buttons.

🧩 Key Functionalities

• TakeImages() → Captures faces and saves them in dataset.
• TrainImages() → Trains the LBPH recognizer with stored images.
• TrackImages() → Detects faces in real time and marks attendance.
• send_email() → Sends attendance CSV via Gmail SMTP.
• delete_registration_csv() / delete_attendance_csv() / delete_registered_images() → Cleans up data.
• change_pass() & save_pass() → Manage admin password securely.

🔐 Security

• Password-protected access for model training.
• Password stored in encrypted form in psd.txt.
• GUI dialog for password change and validation.

📈 Future Improvements

• Integrate database (MySQL/SQLite) for better data management.
• Add real-time dashboard to monitor attendance statistics.
• Replace Haar Cascade with deep learning face embeddings (e.g., FaceNet).
• Deploy as a web app using Flask/Streamlit.
• Add multi-camera support for larger classrooms or offices.

🧾 Deliverables
• Attendance CSV logs
• Student registration dataset
• Tkinter-based executable attendance system

Screenshot:
link:https://github.com/ArchiSaini18/Face-Recognition-Based-Attendance-Monitoring-System-Using-Machine-Learning/blob/main/Screenshot%202025-10-31%20174649.png
