Bus Ticket Booking System
Introduction
Welcome to the Bus Ticket Booking System! This project is a comprehensive graphical user interface (GUI) application built using Java Swing and JDBC. The Bus Ticket Booking System simplifies the process of booking bus tickets through an intuitive and user-friendly interface. With a modern design and essential features, users can easily book, reset, and submit their bus ticket details. The system securely stores booking information in a MySQL database, ensuring that all transactions are both reliable and accurate.

Features
User-Friendly Interface: The application features a clean and simple design, making it easy for users to navigate and book tickets.
Real-Time Database Interaction: Utilizes JDBC to connect to a MySQL database, where all booking data is stored and managed.
Dynamic Date Selection: Users can select their preferred date of departure using an integrated calendar widget.
Flexible Ticket Management: Users can book tickets, reset form details, and submit their booking information with just a few clicks.
Payable Amount Calculation: The system automatically calculates the payable amount based on the number of passengers, ensuring a quick and accurate transaction process.
Technology Stack
Java Swing: Used to create the GUI components such as buttons, text fields, labels, combo boxes, and the calendar widget.
JDBC (Java Database Connectivity): Facilitates the connection between the Java application and the MySQL database.
MySQL: The relational database management system used to store all booking-related data.
Project Structure
Main Components
Booking Form: The main interface where users enter their travel details, including source, destination, departure date, time, and the number of passengers.
Database Connection: The connect() method establishes a connection between the Java application and the MySQL database.
Event Handling: The actionPerformed() method handles user actions, such as booking, resetting, and submitting the form.
Data Insertion: The preparedStatement() method is used to insert booking details into the MySQL database.
SQL Execution: The executeUpdate() method ensures that the booking data is successfully stored by returning the number of affected rows.
Key Methods
connect()
This method establishes a connection between the Java application and the MySQL database. It uses the DriverManager class to connect to the database named busbooking.

actionPerformed()
Handles button click events in the application. It manages the actions associated with the "Submit," "Reset," and "Book" buttons, ensuring the appropriate response is triggered for each user action.

executeUpdate()
This method executes SQL statements that modify the database (such as INSERT, UPDATE, DELETE) and returns the number of rows affected by the execution. It is used to confirm that the ticket booking details have been successfully stored.

preparedStatement()
A method from the java.sql package used to create precompiled SQL statements that can be executed multiple times with different parameters. It is crucial for inserting booking details into the database securely and efficiently.

Getting Started
Prerequisites
Java Development Kit (JDK): Ensure that you have JDK installed on your system.
MySQL Database: Install MySQL and create a database named busbooking to store booking information.
IDE: You can use any Java-supported IDE like IntelliJ IDEA, Eclipse, or NetBeans.
Installation
Clone the repository:

bash
Copy code
git clone https://github.com/your-username/Bus-Ticket-Booking-System.git
Navigate to the project directory:

bash
Copy code
cd Bus-Ticket-Booking-System
Setup the MySQL Database:

Create a database named busbooking.
Import the provided SQL file to set up the necessary tables.
Run the Application:

Open the project in your preferred IDE.
Execute the booking.java file to start the Bus Ticket Booking System.
Usage
Booking a Ticket:

Enter your travel details, including the source, destination, departure date, time, and the number of passengers.
Click the "Book" button to finalize your booking.
Review the ticket summary and payable amount.
Click "Submit" to save the booking details to the database.
Resetting the Form:

Click the "Reset" button to clear all the input fields and start over.
Contributing
Contributions are welcome! If you'd like to contribute to this project, please fork the repository and use a feature branch. Pull requests are encouraged and will be reviewed promptly.

License
This project is licensed under the MIT License - see the LICENSE file for details.

Acknowledgements
Java Swing for providing the powerful GUI components.
JDBC for seamless database connectivity.
The open-source community for the continuous support and resources.
