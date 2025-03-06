# QR Code-Based Attendance System

## Overview
A Python-based attendance system using QR codes, Tkinter, and OpenCV. The system enables teachers to generate QR codes for attendance tracking and allows students to scan them to mark their presence. Attendance records are stored in a CSV file and can be viewed by both teachers and students.

## Features
- **Teacher Login:** Generate QR codes for attendance.
- **Student Login:** Scan QR codes to mark attendance.
- **Attendance Record:** Data is stored in `attendance.csv`.
- **WiFi Verification:** Attendance can only be marked when connected to a specific WiFi.
- **View Attendance:**
  - Teachers can view attendance for all students.
  - Students can view their own attendance records.

## Installation
### Prerequisites
Ensure you have Python installed, then install dependencies:
```bash
pip install -r requirements.txt
```

### Running the Application
To start the system, run:
```bash
python qr.py
```

## Usage
### Teacher Login
1. Enter **User ID** and **Password**.
2. Select a **subject**.
3. Click **Generate QR Code**.
4. Click **View Attendance** to check student records.

### Student Login
1. Enter **User ID** and **Password**.
2. Click **Scan QR Code** to mark attendance.
3. Click **View Attendance** to check personal records.

## Attendance Data Format
The **attendance.csv** file follows this format:
```
Name,DMS,COA,TOC,DBMS,OOPSJ,LMP-2,LOOPSJ,LCOA,LDBMS
Arin,1,0,1,0,0,1,0,1,1
Mayank,1,1,1,0,0,1,1,0,1
```
- **Name:** Student name.
- **Subjects:** Each column represents a subject with the number of attended classes.

## Technologies Used
- **Python**
- **Tkinter** (GUI)
- **OpenCV** (QR Code Scanning)
- **Pandas** (Data Handling)
- **Pillow** (Image Processing)
- **QRCode** (QR Code Generation)
- **Pyzbar** (QR Code Decoding)

## Future Enhancements
- **Database Integration** instead of CSV.
- **Mobile App** version.
- **Email Notifications** for attendance updates.

## License
MIT License

# .gitignore
__pycache__/
qr_codes/
*.pyc
*.pyo
.DS_Store

# requirements.txt
opencv-python
pandas
pyzbar
pillow
qrcode
tkinter
