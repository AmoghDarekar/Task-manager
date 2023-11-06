# Task-manager
Before you begin, make sure you have the following tools and components installed:

1. XAMPP: If you haven't already, download and install XAMPP, which includes Apache, MySQL, and PHP. You can download it here.
2. Text Editor: Install a text editor of your choice. You can use Sublime Text, Visual Studio Code, Atom, or Brackets.
Project Setup:

1. Download this project as a ZIP file or clone it using Git.
2. Move the project folder to the root directory of your XAMPP installation. On a typical Windows installation, this directory is located at Local Disc C: -> xampp -> htdocs -> 'this project'.
3. Open the XAMPP Control Panel and start both the 'Apache' and 'MySQL' services.

Import the Database:
a. Open your web browser and access 'phpMyAdmin'.
b. Create a new database.
c. Import the provided SQL file into your new database.
Configure Settings:
Go to the 'config' folder and open the 'constants.php' file. Make the following changes to the constants:

<?php 
// Start Session
session_start();

// Create Constants to save Database Credentials
define('LOCALHOST', 'localhost');
define('DB_USERNAME', 'root'); // Your Database username (replace 'root')
define('DB_PASSWORD', ''); // Your Database Password (if applicable)
define('DB_NAME', 'task_manager'); // Your Database Name (if different)

define('SITEURL', 'http://localhost/task-manager/'); // Update the project's URL (if needed)
?>

Finally, open the project in your web browser. You should be able to run it smoothly.
