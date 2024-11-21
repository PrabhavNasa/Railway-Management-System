#🚂 Railway Management System
A Java-based Railway Management System leveraging Swing for the GUI and JDBC for database connectivity. This project provides a streamlined and user-friendly platform for managing railway operations, including train schedules, ticket bookings, and passenger information.

📝 Introduction
This project is designed to automate and simplify railway management tasks, ensuring efficiency and user satisfaction.

Key Functionalities
Train Schedule Management
User Login and Registration
Ticket Booking and Cancellation
Passenger Information Management
Admin System Management
⚙️ Features
Train Schedule Management: Add, update, and view train schedules.
User Login and Registration: Secure user authentication system.
Ticket Booking and Cancellation: Real-time ticket management.
Admin Panel: Manage trains, users, and overall system operations.
🖥️ Installation
Prerequisites
Java 8 or higher
MySQL relational database
Steps
Clone the repository:

bash
Copy code
git clone https://github.com/tanishavyastv/railway-management-system.git  
Set up the database:

Install MySQL.
Set username as root and password as 1234.
Create a database named Railway.
Create the required tables:

sql
Copy code
create table train (
    tnum int,
    tname varchar(255),
    seats int,
    bp varchar(255),
    dp varchar(255),
    fAC int,
    sAC int,
    tAC int,
    sc int,
    doj date,
    atime varchar(20),
    dtime varchar(20),
    sno int PRIMARY KEY auto_increment
);

create table user (
    uname varchar(10),
    pass varchar(10),
    age int,
    g varchar(10),
    sno int PRIMARY KEY auto_increment
);

create table chart (
    sno int PRIMARY KEY auto_increment,
    ticketID varchar(10),
    tnum int,
    pnr varchar(20),
    name varchar(20),
    age int,
    gender varchar(10),
    seatno int,
    coach varchar(20),
    dot date
);
🚀 Running the Application
Using an IDE
Visual Studio Code (VSCode)
Open the railway-management-system folder.
Navigate to the Railway.java file.
Right-click and select Run Java.
NetBeans
Import the folder as a project in NetBeans.
Locate Railway.java in the Projects panel.
Right-click and select Run File.
Eclipse
Open the folder as a project in Eclipse.
Locate Railway.java in the Package Explorer.
Right-click and select Run As > Java Application.
📸 Application Screenshots
