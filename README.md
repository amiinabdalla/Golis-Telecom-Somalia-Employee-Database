# Golis Telecom - HR & Employee Management Database System

## 📌 Overview
This project is a relational database system designed for **Golis Telecom** to manage company operations, staff details, structural hierarchy, payroll processing, and daily attendance. 

The schema is normalized to ensure data integrity, eliminate redundancy, and maintain proper relational mapping between entities.

---

## 🏗️ Database Architecture & Schema Structure

The database consists of **6 primary tables**:

1. **`Departments`**: Stores department details within the company.
2. **`Branches`**: Tracks different Golis Telecom company locations/cities.
3. **`Positions`**: Defines employee job titles and roles.
4. **`Employees`**: Central table containing personal, contact, structural assignment details, and active status.
5. **`Salaries`**: Manages monthly payroll records including base salary, allowances, deductions, and net salary calculations.
6. **`Attendance`**: Tracks daily employee attendance logs and work statuses.

---

## 🔗 Entity Relationships (ERD Mapping)

- **`Employees` ➔ `Departments`** *(Many-to-One)*: An employee belongs to one department.
- **`Employees` ➔ `Branches`** *(Many-to-One)*: An employee works at a specific branch.
- **`Employees` ➔ `Positions`** *(Many-to-One)*: An employee holds a specific job title.
- **`Employees` ➔ `Salaries`** *(One-to-Many)*: An employee can have multiple monthly salary records.
- **`Employees` ➔ `Attendance`** *(One-to-Many)*: An employee has multiple attendance logs over time.

---

## 🛠️ Tech Stack & Features
- **Database Engine:** SQL (MySQL / PostgreSQL / MS SQL Server)
- **Design Standards:** 3NF Normalization, Foreign Key Constraints (`NN` / `NOT NULL`), Relational Integrity
- **Key Modules:** HR Management, Multi-branch Operations, Automated Payroll Tracking, Attendance Monitoring

---

## 🚀 How to Use
1. Clone the repository:
   ```bash
   git clone [https://github.com/your-username/golis-telecom-database.git](https://github.com/your-username/golis-telecom-database.git)
