# ClassMate - Student Management System

## Overview
ClassMate is a web-based Student Management System built using Flask and MySQL. It helps educational institutions efficiently manage student data, courses, attendance, and performance records in an easy-to-use interface.

## Features
- **Student Management**: Add, update, and delete student records.
- **Course Management**: Assign students to courses and track enrollments.
- **Attendance Tracking**: Mark and monitor student attendance.
- **Grades & Performance**: Record and evaluate student grades.
- **User Authentication**: Secure login system with role-based access (Admin, Teacher, Student).
- **Dashboard & Reports**: Visual summaries of student progress and attendance.

## Technologies Used
- **Backend**: Flask (Python)
- **Frontend**: HTML, CSS, JavaScript (Bootstrap for styling)
- **Database**: MySQL
- **ORM**: SQLAlchemy
- **Authentication**: Flask-Login

## Installation
### Prerequisites
Ensure you have the following installed:
- Python (>= 3.7)
- MySQL
- Virtualenv (optional but recommended)

### Setup Steps
1. **Clone the Repository**
   ```sh
   git clone https://github.com/yourusername/classmate.git
   cd classmate
   ```
2. **Create a Virtual Environment** (optional but recommended)
   ```sh
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```
3. **Install Dependencies**
   ```sh
   pip install -r requirements.txt
   ```
4. **Set Up MySQL Database**
   - Create a MySQL database:
     ```sql
     CREATE DATABASE classmate_db;
     ```
   - Update `config.py` with your MySQL credentials.
   
5. **Run Database Migrations**
   ```sh
   flask db init
   flask db migrate -m "Initial migration."
   flask db upgrade
   ```
6. **Run the Application**
   ```sh
   flask run
   ```
   The app will be available at `http://127.0.0.1:5000/`.

## Usage
- **Admin** can manage users, courses, and student records.
- **Teachers** can mark attendance and update grades.
- **Students** can view their progress and enrolled courses.

## Contribution
Feel free to fork this repository, raise issues, or submit pull requests.

## License
This project is licensed under the MIT License.

## Contact
For any issues or suggestions, reach out at navyajinayak2003@gmail.com or open an issue on GitHub.

