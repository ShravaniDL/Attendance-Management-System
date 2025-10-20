# Attendance-Management-System
The Attendance Management System is a digital way to take attendance. It keeps a student database with name, ID, class, and contact. Teachers can mark attendance fast, and it saves the date and time. It makes daily, weekly, and monthly reports. Parents get alerts about absence, holidays, and timetables. 
<br>
author - Shravani D L 
1. Setup (First Time)
Sign up as an Admin use
<br>
The system will automatically create default classes
Navigate to "Classes" to view or modify classes
3. Add Students
Go to "Students" section
Click "+ Add Student"
Fill in student details and select a class from the dropdown
Save the student
4. Mark Attendance
Go to "Attendance" section
Select a date and class
Mark students as Present/Absent/Leave using radio buttons
Click "Save" to record attendance
5. View Reports
Go to "Reports" section
Select class, date range, and date
Click "Run" to generate attendance reports
User Roles
Admin: Full access to all features
Teacher: Can manage students, classes, and attendance
Student/Parent: Read-only access
Technical Details
Database Structure
/users/{uid} - User profiles and roles
/classes/{classId} - Class information
/students/{studentId} - Student records
/attendance/{date}/class_{classId}/{studentId} - Attendance records
/holidays/{holidayId} - Holiday calendar
/timetable/{classId} - Class timetables
Key Fixes Applied
Added missing classes management functionality
Fixed student-class relationship with proper dropdowns
Improved error handling in attendance saving
Added default data creation for new installations
Enhanced UI with better styling and feedback
Running the Application
Ensure Firebase is properly configured in public/script.js
Serve the files using a local server:
python -m http.server 8000
# or
npx serve public
Open http://localhost:8000 in your browser
Firebase Configuration
Make sure your Firebase project has:

Authentication enabled (Email/Password)
Firestore Database enabled
Proper security rules (included in firestore.rules)
The attendance system is now fully functional and ready for use!
