# Attendance-Management-System
The Attendance Management System is a digital way to take attendance. It keeps a student database with name, ID, class, and contact. Teachers can mark attendance fast, and it saves the date and time. It makes daily, weekly, and monthly reports. Parents get alerts about absence, holidays, and timetables. 
<br>
author - Shravani D L 
# 🧾 Attendance Management System

A simple web-based Attendance Management System built using **Firebase** for real-time data handling and user authentication.

---

## ⚙️ 1. Setup (First Time)
- Sign up as an **Admin user**<br>
- The system will automatically create default classes<br>
- Navigate to **"Classes"** to view or modify classes<br>

---

## 👩‍🎓 2. Add Students
- Go to **"Students"** section<br>
- Click **"+ Add Student"**<br>
- Fill in student details and select a class from the dropdown<br>
- Click **Save** to add the student<br>

---

## 📋 3. Mark Attendance
- Go to **"Attendance"** section<br>
- Select a **date** and **class**<br>
- Mark students as **Present / Absent / Leave** using radio buttons<br>
- Click **Save** to record attendance<br>

---

## 📊 4. View Reports
- Go to **"Reports"** section<br>
- Select **class**, **date range**, and **date**<br>
- Click **"Run"** to generate attendance reports<br>

---

## 👥 User Roles
- **Admin:** Full access to all features<br>
- **Teacher:** Can manage students, classes, and attendance<br>
- **Student / Parent:** Read-only access<br>

---

## 🧩 Technical Details

### 🗄️ Database Structure
/users/{uid} - User profiles and roles
/classes/{classId} - Class information
/students/{studentId} - Student records
/attendance/{date}/class_{classId}/{studentId} - Attendance records
/holidays/{holidayId} - Holiday calendar
/timetable/{classId} - Class timetables

