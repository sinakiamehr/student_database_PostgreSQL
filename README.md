# 🎓 FreeCodeCamp: PostgreSQL Student-Course Database

This project is part of the **FreeCodeCamp Relational Database Certification**, focused on learning PostgreSQL by designing and querying a simple relational database involving students and courses.

## 📁 Project Contents

- 📁 Inserting Data
-- `student.csv` – CSV file containing student data.
-- `courses.csv` – CSV file containing course information.
-- `students.sql` – SQL file used to create the database schema and tables.
-- `insert_data.sh` – Bash script used to import CSV data into the database using `psql`.

---

## 🧰 Requirements

- PostgreSQL (version 13 or later recommended)
- `psql` command-line tool
- Unix-like environment (macOS, Linux, or WSL/Git Bash)

---

## 🏗️ Database Structure

The schema defined in `students.sql` creates two main tables:

### 📄 `student`
| Column         | Type         | Description               |
|----------------|--------------|---------------------------|
| student_id     | SERIAL       | Primary key               |
| name           | TEXT         | Full name of the student  |
| email          | TEXT         | Unique email address      |
| enrollment_date| DATE         | Date of enrollment        |

### 📄 `course`
| Column     | Type     | Description            |
|------------|----------|------------------------|
| course_id  | SERIAL   | Primary key            |
| title      | TEXT     | Course title           |
| credits    | INTEGER  | Number of credit hours |

---

## 🚀 How to Run the Project

### 1. 🛠️ Set Up PostgreSQL
Make sure PostgreSQL is installed and the `psql` CLI is available.

### 2. 📂 Clone or Copy Files

Place all files in a single working directory (e.g., `postgres-students`).

### 3. 🏗️ Create the Database

```bash
createdb students
