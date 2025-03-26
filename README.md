# Sign-Up and Login System
A simple web-based Sign-Up and Login system built using HTML, CSS, JavaScript, PHP, and MySQL.

## 📌 Overview
This project is a Sign-Up and Login system that allows users to create accounts and log in securely. It includes basic form validation, password hashing, and responsive UI for a seamless user experience. The project uses MySQL to store user details and supports basic user authentication.

## ✨ Features

### 🔐 Account Management
- ✅ **User Registration** (Username, Firstname, Lastname, Password)
- 🔑 **Secure Login** (Username + Password)
- 👤 **Account Validation** (Input validation for empty fields and password length)

### 💼 User Interface
- 💻 **Responsive UI** (Mobile-friendly form layout)
- 🎨 **Styled Forms** (Custom styling with CSS for a modern look)

### 🛡️ Security & Validation
- 🔒 **Password Hashing** (Securely stores passwords using MD5 hashing)
- 📝 **Client-Side Form Validation** (Uses JavaScript to ensure valid user input)
- 📂 **Database Storage** (User details are stored in a MySQL database)

## 🛠️ How to Run

### Prerequisites
- A local server (e.g., XAMPP, WAMP)
- A MySQL database

### Setup Instructions

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/sign-up-login-system.git
    cd sign-up-login-system
    ```

2. Database Setup:
    - Create a MySQL database named `User_database`.
    - Run the following SQL to create a table:
    ```sql
    CREATE TABLE users (
        id INT AUTO_INCREMENT PRIMARY KEY,
        firstname VARCHAR(50) NOT NULL,
        lastname VARCHAR(50) NOT NULL,
        username VARCHAR(50) NOT NULL UNIQUE,
        password VARCHAR(255) NOT NULL
    );
    ```

3. Update the database credentials in the `register.php` and `login.php` files.

4. Start your local server (XAMPP/WAMP) and place the project files in the `htdocs` (XAMPP) or `www` (WAMP) directory.

5. Open `http://localhost/sign-up-login-system/index.html` in your browser.

## 📂 File Structure
- `index.html` → Login Page
- `register.html` → Registration Page
- `Form.css` → Stylesheet for the forms
- `validate.js` → Client-side form validation script
- `register.php` → Handles user registration (stores data in the database)
- `login.php` → Handles user login (validates user credentials)
- `avatar.png` → Sample user avatar for display
- `form.jpg` → Background image for the form page

## 📜 Code Structure
- **HTML** → Provides the structure for the login and registration forms
- **CSS** → Styles the forms and UI elements
- **JavaScript** → Handles client-side form validation
- **PHP** → Processes form data, connects to the MySQL database, and stores/retrieves user details
- **MySQL** → Used for storing user data in the `users` table

## 🤝 Contributing
Feel free to fork the repository, suggest improvements, and submit pull requests!

### Possible Improvements:
- Use `password_hash()` for more secure password hashing.
- Add email verification functionality.
- Enhance UI/UX with frameworks like Bootstrap.

## 📜 License
This project is licensed under the [MIT License].

🌟 Enjoy creating your account and logging in securely! 🔒💻

