# Doctor Appointment System – PHP

A web-based Doctor Appointment System developed using **PHP, MySQL, HTML, CSS, and JavaScript**. The system provides an online platform for patients to find doctors and book appointments while allowing doctors and administrators to manage appointment-related information.

## Project Overview

The Doctor Appointment System is designed to simplify the traditional appointment-booking process. Patients can register on the system, view doctors, and book appointments according to availability.

The system also provides facilities for managing doctors, patients, appointments, and related records through a centralized database.

## Objectives

* Provide an online doctor appointment booking facility.
* Reduce manual appointment scheduling.
* Maintain patient and doctor information digitally.
* Reduce appointment scheduling errors.
* Improve accessibility for patients.
* Simplify appointment management for doctors and administrators.
* Store system information securely in a MySQL database.

## Main Modules

### 1. Patient Module

The patient module allows users to:

* Register an account.
* Log in to the system.
* View available doctors.
* Select a doctor.
* Book an appointment.
* View appointment information.
* Manage their basic information.

### 2. Doctor Module

The doctor module allows doctors to:

* Log in to the system.
* View scheduled appointments.
* Manage appointment information.
* View relevant patient information.
* Manage their availability.

### 3. Admin Module

The administrator module provides management facilities for:

* Doctors
* Patients
* Appointments
* User accounts
* System records

## Technologies Used

| Technology | Purpose                       |
| ---------- | ----------------------------- |
| PHP        | Backend development           |
| HTML       | Web page structure            |
| CSS        | Interface styling             |
| JavaScript | Client-side functionality     |
| MySQL      | Database management           |
| Apache     | Web server                    |
| XAMPP/WAMP | Local development environment |

## System Requirements

### Hardware Requirements

* Intel Core i3/i5 processor or equivalent
* 4 GB / 8 GB RAM
* 512 GB / 1 TB hard disk
* 15.6-inch monitor or better
* Keyboard and mouse

### Software Requirements

* Windows 10 / Windows 11
* XAMPP or WAMP
* Apache Web Server
* MySQL
* PHP
* Google Chrome, Mozilla Firefox, or another suitable browser

## Project Structure

```text
Doctor-Appointment-System_PHP/
│
├── admin/
│   ├── dashboard.php
│   ├── doctors.php
│   ├── patients.php
│   └── appointments.php
│
├── doctor/
│   ├── dashboard.php
│   ├── appointments.php
│   └── profile.php
│
├── patient/
│   ├── dashboard.php
│   ├── doctors.php
│   ├── book-appointment.php
│   └── appointments.php
│
├── assets/
│   ├── css/
│   ├── js/
│   └── images/
│
├── config/
│   └── database.php
│
├── includes/
│   ├── header.php
│   ├── footer.php
│   └── auth.php
│
├── index.php
├── login.php
├── register.php
├── logout.php
└── database.sql
```

## Database

The project uses **MySQL** for storing application data.

Important entities include:

* Doctors
* Patients
* Users
* Appointments

Example doctor information includes a unique doctor ID, name, and email. The project documentation specifies the doctor ID as an auto-incrementing primary key and the doctor's name as a required field.

## Installation

### Step 1 – Install XAMPP

Install XAMPP on your computer and start:

```text
Apache
MySQL
```

### Step 2 – Copy the Project

Copy the project folder into:

```text
C:\xampp\htdocs\
```

For example:

```text
C:\xampp\htdocs\Doctor-Appointment-System_PHP
```

### Step 3 – Create the Database

Open:

```text
http://localhost/phpmyadmin
```

Create a new database, for example:

```text
doctor_appointment
```

Import the provided:

```text
database.sql
```

file into the database.

### Step 4 – Configure Database Connection

Update the database configuration file with your MySQL credentials.

Example:

```php
<?php

$host = "localhost";
$username = "root";
$password = "";
$database = "doctor_appointment";

$conn = mysqli_connect(
    $host,
    $username,
    $password,
    $database
);

if (!$conn) {
    die("Database connection failed: " . mysqli_connect_error());
}

?>
```

### Step 5 – Run the Project

Open your browser and visit:

```text
http://localhost/Doctor-Appointment-System_PHP/
```

## Project Advantages

* Online appointment booking
* Reduces manual administrative work
* Provides easier access to doctors
* Helps organize appointment records
* Reduces scheduling errors
* Provides centralized information management
* Allows patients to book appointments conveniently

## Limitations

* Requires internet/network or local server availability.
* Users need basic digital literacy.
* Patient information requires strong security measures.
* System reliability depends on server and database availability.
* Incorrect doctor availability information could result in scheduling problems.

The project documentation also identifies technological barriers, privacy/security concerns, overbooking, system reliability, and reduced personal interaction as potential disadvantages.

## Future Enhancements

Possible future improvements include:

* Email and SMS appointment notifications
* Online payment integration
* Video consultation
* Prescription management
* Electronic medical records
* Doctor search and filtering
* Appointment reminders
* Role-based access control
* Two-factor authentication
* Responsive mobile interface
* Advanced reporting and analytics

## Project Documentation

The project includes documentation covering:

* Feasibility Study
* Requirement Gathering and Analysis
* Software Requirements Specification
* Hardware Requirements
* Software Requirements
* Class Diagram
* Entity-Relationship Diagram
* Sequence Diagram
* Use Case Diagram
* System Flow Diagram
* Data Dictionary
* 0-Level DFD
* 1-Level DFD
* Level-2 DFD
* Activity Diagram

## Team Members

* **Sudarshan Sinha** – 2305103140031
* **Krishna Shankar** – 2305103140018
* **Suparna Das** – 2305103140032

## License

This project is developed for academic/educational purposes.
