Task 2: Data Types, Constraints & Table Design
🔹 Internship: SQL Developer Internship
🔹 Task Name: Data Types, Constraints & Table Design

🛠️ Tools Used

MySQL Workbench

MySQL (XAMPP)

📂 Table Description

A students table was designed using appropriate data types and constraints such as:

PRIMARY KEY

NOT NULL

UNIQUE

AUTO_INCREMENT

🧱 Table Creation
CREATE TABLE students (
    student_id INT PRIMARY KEY AUTO_INCREMENT,
    name VARCHAR(100) NOT NULL,
    email VARCHAR(100) UNIQUE NOT NULL,
    date_of_birth DATE NOT NULL,
    gender CHAR(1),
    department VARCHAR(50) NOT NULL,
    admission_date DATE NOT NULL
);

🧪 Data Insertion
Valid Data
INSERT INTO students (name, email, date_of_birth, gender, department, admission_date)
VALUES ('Nithya', 'nithya@gmail.com', '2003-12-11', 'F', 'CSE', '2022-08-01');

🔧 Table Alterations
Add a New Column
ALTER TABLE students
ADD phone_number VARCHAR(15);

Rename a Column
ALTER TABLE students
RENAME COLUMN phone_number TO mobile_number;

Drop a Column
ALTER TABLE students
DROP COLUMN gender;


⚠️ Dropping a column permanently deletes the data.

🎯 Constraints Explanation
Constraint	Purpose
PRIMARY KEY	Uniquely identifies records
NOT NULL	Prevents missing values
UNIQUE	Avoids duplicate entries
AUTO_INCREMENT	Generates IDs automatically
