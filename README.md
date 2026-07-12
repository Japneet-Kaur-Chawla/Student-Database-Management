# Student Database Management System (Pure SQL)

## 📌 About the Project
This project is a lightweight, fully relational Student Database Management System designed using standard Oracle SQL. 

Rather than relying on heavy PL/SQL components like Triggers or Views, this architecture focuses strictly on core database fundamentals: robust table design, strict data integrity constraints, and dynamic data retrieval using advanced `SELECT` queries. It models a real-world academic environment, handling everything from student enrollments to attendance tracking and fee management.

## 🏗️ Database Schema Overview
The relational database consists of 8 interconnected tables:
* **Departments:** Manages academic departments.
* **Instructors:** Stores faculty details and links them to departments.
* **Students:** Tracks student profiles and enrollment years.
* **Semesters:** Manages academic terms and date ranges.
* **Courses:** Defines classes, credit limits, and assigned instructors.
* **Enrollments:** Connects students to courses per semester and stores academic marks.
* **Attendance:** Tracks daily student presence (Present, Absent, Late).
* **Fees:** Manages financial billing, tracking amounts due versus amounts paid.

## 🚀 Key Technical Concepts Demonstrated
* **Relational Mapping:** Extensive use of Primary Keys (PK) and Foreign Keys (FK) to establish 1-to-Many and Many-to-Many relationships.
* **Data Integrity:** Implementation of `CHECK`, `UNIQUE`, and `NOT NULL` constraints to prevent bad data entry (e.g., ensuring marks stay between 0 and 100).
* **Automated Indexing:** Strategic use of `CREATE INDEX` on foreign keys to optimize query performance during multi-table joins.
* **Dynamic Calculations:** Use of `CASE` statements to calculate alphabetical grades and financial statuses on the fly, eliminating the need for stored triggers.
* **Advanced Querying:** Complex `JOIN` operations, aggregate functions (`AVG`, `COUNT`), and `GROUP BY` clauses to generate real-time analytical reports.

---

## 🛠️ How to Run the Project (For Interviewers)

This script was written for **Oracle Database 12c+**, utilizing `IDENTITY` columns for auto-incrementing primary keys. You can run this in Oracle SQL Developer, Oracle Live SQL (web-based), or any compatible SQL client.

### Step 1: Clone the Repository
Open your terminal and run the following command to pull the code to your local machine:
```bash
git clone [https://github.com/Japneet-Kaur-Chawla/Student-Database-Management.git](https://github.com/Japneet-Kaur-Chawla/Student-Database-Management.git)
cd Student-Database-Management
```

### Step 1: Prepare the Environment
1. Open your Oracle SQL environment.
2. Open a new SQL worksheet.

### Step 2: Build the Schema
1. Copy the contents of the `code.sql` file (or paste the single-file script).
2. Run the script from top to bottom. 
> **Note:** The script begins with a series of `DROP TABLE` commands to ensure a clean slate. If this is your first time running it, you will see "table or view does not exist" errors for the drop commands—these are expected and can be safely ignored.

---
*Developed as a portfolio project to demonstrate proficiency in SQL database design and data analysis.*