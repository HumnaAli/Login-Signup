# Login-Signup Page
Login System Project
The Login System project is a graphical user interface (GUI) application developed in Python using the Tkinter library. It provides users with the ability to sign up for an account, securely store their credentials in an SQLite database, and log in to their accounts.

Features
The application offers the following features:

Sign up: Users can create a new account by providing a unique username and password. The password is securely hashed using the bcrypt library before being stored in the database.
Login: Existing users can log in to their accounts by entering their username and password. The application compares the entered credentials with the hashed password stored in the database for authentication.
User Interface: The application provides an intuitive and visually appealing user interface with appropriate labels, buttons, and entry fields.
Technologies Used
The Login System project utilizes the following technologies:

Python: The programming language used for developing the application.
Tkinter: The standard Python interface to the Tk GUI toolkit for creating the graphical user interface.
SQLite: A lightweight, file-based relational database management system used for storing user credentials.
bcrypt: A library used for secure password hashing.
Dependencies
To run the application, the following libraries and modules are required:

Tkinter: Installable via pip (pip install tk).
Pillow: Installable via pip (pip install pillow).
bcrypt: Installable via pip (pip install bcrypt).
Implementation Details
The implementation of the Login System project involves the following steps:

Import Required Modules: Necessary modules and libraries such as Tkinter, customtkinter, SQLite, bcrypt, messagebox from tkinter, PIL (Python Imaging Library), and os are imported.

Set Up Application: An instance of the customtkinter.CTk class is created as the main application window. The window is configured with a title, dimensions, and background color.

Define Fonts: Different fonts are defined using tuples to specify font properties.

Set Up Database: A connection is established with the SQLite database file named "data.db". A cursor object is created to execute SQL statements.

Create Users Table: A table named "users" is created in the database if it doesn't exist. The table has two columns: "username" and "password".

Implement Sign Up Function: The signup() function is defined to handle the sign-up functionality. It retrieves the entered username and password from the respective entry fields. If the fields are not empty, it checks if the username already exists in the database. If not, the password is hashed using bcrypt, and the username and hashed password are inserted into the "users" table. A success message is displayed if the account is created successfully; otherwise, an error message is shown.

Implement Login Account Function: The login_account() function handles the login functionality. It retrieves the entered username and password from the respective entry fields. If the fields are not empty, it retrieves the hashed password from the database for the given username. If a result is found, it compares the entered password with the hashed password using bcrypt. If they match, a success message is displayed; otherwise, an error message is shown.

Implement Login Function: The login() function is called when the "Login" button is clicked. It destroys the initial sign-up frame and creates a new frame for the login screen. It sets up a label, entry fields, and a login button in the new frame. The login button is linked to the login_account() function.

Create Sign Up Frame: The initial sign-up frame is created using the customtkinter.CTkFrame class. Labels, entry fields, and a sign-up button are placed in t
zhe frame. The sign-up button is linked


<img width="288" alt="image" src="https://github.com/HumnaAli/Login-Signup/assets/100784745/0579dbc1-df4b-4fe5-be5c-3918b9545234">
<img width="289" alt="image" src="https://github.com/HumnaAli/Login-Signup/assets/100784745/4f1f3c62-47d4-4902-8dc3-3ef06fa9e129">



