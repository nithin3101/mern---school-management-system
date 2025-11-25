# School Management System – MERN

<p> A full-stack School Management System built using the MERN stack (MongoDB, Express.js, React.js, Node.js) and structured using the MVC architecture.
 This system digitalizes student management, teacher assignment, attendance, marks, and announcements.
</p>

## Key Features
* Secure role-based authentication for Admin, Teacher, and Student (JWT).
* Auto dashboard redirection after login.
* Admin: manage students, teachers, classes, subjects, announcements, attendance & marks reports.
* Teacher: take attendance, update marks, view class lists, post announcements.
* Student: view profile, subjects, marks, attendance, timetable, announcements.

## Architecture – MVC Pattern

The system follows the MVC architectural pattern:

- **Model**  
  Handles database schemas and data logic  
  (Students, Teachers, Subjects, Classes, Attendance, Marks)

- **View**  
  React.js front-end  
  (Builds UI for each role dashboard)

- **Controller**  
  Node.js + Express.js  
  (Handles requests, validation, business logic)

## Tech Stack

### **Frontend**
- React.js  
- Axios  
- React Router  
- CSS / Bootstrap / Material UI  

### **Backend**
- Node.js  
- Express.js  
- JWT Authentication  
- MVC Pattern  

### **Database**
- MongoDB (Mongoose ORM)

## Installation & Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/nithin3101/mern---school-management-system.git
   cd School-Management-System
   ```
   
2. Install Backend Dependencies
   ```bash
   cd backend
   npm install
   ```

3. Install Frontend Dependencies
   ```bash
   cd frontend
   npm install
   ``` 
4. Create a `.env` file inside backend
   ```bash
   MONGO_URI=your_mongodb_connection_string
   JWT_SECRET=your_secret_key
   PORT=5000
   ```

5. Start Backend Server
   ```bash
   cd backend
   npm start
   ```

6. Start Frontend Server
   ```bash
   cd frontend
   npm start
   ```
## API Endpoints

### Auth API  
- `POST` `/api/auth/login`  – User login
- `GET` `/api/auth/me` - Get current user
- `POST` `/api/auth/logout` - User logout

### Student API 
- `GET` `/students` – Get all students  
- `POST` `/students` – Add new student
- `PUT` `/students/:id` – Update student
- `DELETE` `/students/:id` – Delete student

### Teacher API
- `GET` `/teachers` – Get all teachers
- `POST` `/teachers` – Add new teacher
- `PUT` `/teachers/:id` – Update teacher
- `DELETE` `/teachers/:id` – Delete teacher

### Attendance API
- `POST` `/attendance` – Mark attendance
- `GET` `/attendance/:classId` – Get attendance by class

### Marks API
- `POST` `/marks` – Add marks
- `GET` `/marks/:studentId` – Get student marks


### Announcement API
- `POST` `/announcements` – Create announcement
- `GET` `/announcements` – Get announcements

## Conclusion
This School Management System demonstrates an efficient and scalable MERN-based solution designed to digitalize school operations.




