# User Authentication and Social Feed

## Project Overview
It is a web-based application that provides user authentication (sign-up and login) and a basic social feed where users can view posts. The project includes HTML, CSS, JavaScript for front-end validation, and PHP with MySQL for backend authentication.

## Features
- User Registration
- User Login with validation
- Password hashing (MD5 - Note: Should be updated to a more secure hashing method like bcrypt)
- User authentication with database verification
- Social media-style feed with dummy posts
- Responsive UI

## Technologies Used
- HTML, CSS, JavaScript (Frontend)
- PHP (Backend)
- MySQL (Database)

## File Structure
```
│── index.html         # Login page
│── register.html      # Registration page
│── home.php           # User home feed page
│── Form.css           # Styling for forms
│── validate.js        # Frontend validation
│── login.php          # Handles user login
│── register.php       # Handles user registration
│── database.sql       # Database schema
```

## Setup Instructions
### Prerequisites:
- Install XAMPP or any local PHP server
- MySQL database

### Steps to Run
1. Clone the repository:
   ```sh
   git clone https://github.com/your-username/EMIGO.git
   ```
2. Start your XAMPP (Apache and MySQL services)
3. Import `database.sql` into MySQL
4. Configure database connection in `login.php` and `register.php`
5. Run the project on `localhost`

## Security Notes
- MD5 hashing is insecure; use bcrypt or password_hash() instead.
- Implement prepared statements to prevent SQL Injection.

## Future Improvements
- Add email verification for sign-ups
- Use sessions for login authentication
- Implement profile page for users

## Author
- Nirajan Chaudhary
- email= nirajanchaudhary624@gmail.com

