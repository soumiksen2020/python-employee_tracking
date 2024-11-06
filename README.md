# Employee Tracking Application

This repository contains a Python application for tracking employee application usage and taking periodic screenshots. It generates a report of application usage and saves it in a Word document.

## Table of Contents

- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [License](#license)

## Prerequisites

Before running this application, ensure you have the following installed on your system:

1. **Python** (version 3.6 or higher)
2. **Pip** (Python package installer)
3. **MySQL** (for the database)

### Installing Python

1. **Download Python**:
   - Go to the [official Python website](https://www.python.org/downloads/).
   - Download the latest version of Python for your operating system.

2. **Install Python**:
   - Run the installer and ensure you check the box that says "Add Python to PATH".
   - Follow the installation instructions.

3. **Verify Installation**:
   - Open your command prompt or terminal and run:
     ```bash
     python --version
     ```
   - You should see the Python version number.

## Installation

1. **Clone the Repository**:
   Open your command prompt or terminal and run:
   ```bash
   git clone https://github.com/soumiksen2020/python-employee_tracking.git
   cd python-employee_tracking

## install the required libraries with the following commands:

pip install pymysql pyautogui pystray Pillow python-docx matplotlib numpy

## Set Up MySQL Database:

Install MySQL and set it up on your machine.
Create a database named usage_tracker.
Create the necessary tables (applications and work_logs) in your database. You can use the following SQL commands:

CREATE TABLE applications (
    app_name VARCHAR(255),
    start_time DATETIME,
    end_time DATETIME,
    duration INT
);

CREATE TABLE work_logs (
    id INT AUTO_INCREMENT PRIMARY KEY,
    start_time DATETIME,
    end_time DATETIME
);

## Run the Application
1. pyinstaller --onefile --windowed --hidden-import=pymysql --hidden-import=docx E:\app_monitor.py
( since my python file is in E: )
2. app_monitor.exe

## Using the System Tray Icon:
Once the application is running, an icon will appear in your system tray.
Right-click the icon to see options for starting and stopping tracking, as well as exiting the application.

## Generate Report:
When you stop the tracking, the application will automatically generate a Word report summarizing the application usage.
The report will get generated in the 'dist' folder as can be seen in the below screnshot.

## Screenshot:
![image](https://github.com/user-attachments/assets/b62251be-aa0b-42e1-91b6-2a3a24ce4dea)




