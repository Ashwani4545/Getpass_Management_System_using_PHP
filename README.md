Gate Pass Management System (GPMS)
This project is a simple web-based application for managing gate passes. It's built with PHP and uses a MySQL database for storing and retrieving pass information. The system features an administrator-only interface to handle the creation, modification, and deletion of gate passes, as well as a dashboard for a quick overview of pass activity.

🚀 Features
Secure Admin Login: A dedicated login page for administrators to access the system.

Dynamic Dashboard: The dashboard provides key statistics, including the total number of passes, passes created today, and passes created in the last 7 days.

CRUD Operations: Administrators can create new passes, view pass details, edit existing pass information, and delete passes.

Automatic Pass Number Generation: New passes are assigned a unique, randomly generated 9-digit pass number.

Print Functionality: A dedicated feature allows for printing a pass from its details page.

Responsive Design: The interface uses Bootstrap 5.3 for a modern and mobile-friendly layout.

🛠️ Prerequisites
To run this project, you will need a local or remote web server environment with the following components:

Web Server: Apache

PHP: Version 7.2.1 or higher.

Database: MySQL or MariaDB.

Dependencies: The project uses Bootstrap 5.3 and Font Awesome icons, which are loaded via CDN in the provided code.

⚙️ Installation and Setup
Follow these steps to get the project up and running on your local machine.

1. Database Setup
First, you need to create the database and its tables.

Open your database management tool (e.g., phpMyAdmin, MySQL Workbench).

Create a new database named getpassdb.

Import the getpassdb.sql file into the newly created database. This will create the necessary admin and passes tables and populate them with initial data.

2. Configure Database Connection
Next, update the database connection details.

Open the db.php file in a text editor.

Modify the DB_SERVER, DB_USERNAME, and DB_PASSWORD constants with your local database credentials. The DB_NAME should remain getpassdb.

3. Deploy Project Files
Place all the project files in your web server's root directory (e.g., htdocs/ for XAMPP or www/ for WAMP).

4. Admin Credentials
The initial database dump provides a default administrator account for testing:

Username: admin

Password: admin (the MD5 hash 21232f297a57a5a743894a0e4a801fc3 is stored in the database).

🖥️ Usage
Navigate to the index.php file in your web browser (e.g., http://localhost/index.php).

Log in using the provided admin credentials.

After logging in, you will be redirected to the dashboard, where you can view pass statistics.

Use the navigation links (which would typically be included via includes/sidebar.php and includes/header.php) to access different sections like Add Pass, Manage Passes, and Logout.
