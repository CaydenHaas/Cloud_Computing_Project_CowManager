#Cow Manager Application
Overview
Cow Manager is a full-stack web application designed to help users efficiently manage their cattle and user accounts. The application includes features for signing up, signing in, managing cows, and viewing user profiles. This README outlines the architecture, security measures, and user guidelines for interacting with the application.

User Guidelines

Getting Started

Sign Up:
Navigate to the Sign-Up page from the home screen.
Provide your name, email, password, address, and phone number.
Upon successful registration, you will be redirected to the Sign-In page.

Sign In:
Enter your registered email and password.
Upon successful authentication, you will be redirected to your profile page.

Managing Cows:
Use the cow management dashboard to add, update, or delete cow records.
Each cow has attributes such as Cow ID, Age, Breed, Date of Ownership, and Number of Offspring.

Profile:

View your profile details.
Log out securely when you are done.

Project Architecture

Frontend
Framework: React.js
Routing: React Router for seamless navigation.
State Management: React's useState and useEffect hooks.

Key Components:
Landing Page: The entry point with navigation options.
SignUp Page: Handles user registration.
SignIn Page: Authenticates existing users.
Profile Page: Displays user details and allows logging out.
CowForm: Form for adding or updating cow data.

Backend
Framework: Node.js with Express.js.
Database: PostgreSQL using Sequelize ORM.
API Endpoints:
/api/users: Handles user registration.
/api/users/auth: Authenticates users.
/api/cows: Manages cow data (CRUD operations).

Security Measures:
Input validation to ensure only valid data is processed.
Passwords stored in plain text for simplicity during development (to be replaced with hashing in production).
Middleware for handling errors and logging.
Security Highlights

CORS:

Configured to allow requests between frontend and backend on different origins.
Middleware: cors.
Input Validation:

Frontend and backend validate required fields (e.g., email, password).
Password Handling:

Currently stored in plain text for simplicity.
Future improvements include implementing password hashing with bcrypt and using JWT for authentication.
Error Handling:

Clear error messages for debugging.
Error codes returned for client-side interpretation (e.g., 401 for unauthorized access, 404 for not found).
User Workflow
Sign-Up Process
Navigate to the Sign-Up page.
Fill in all required fields.
Submit the form to create your account.
Sign-In Process
Navigate to the Sign-In page.
Enter your email and password.
Access your profile upon successful authentication.
Managing Cows
Add cows:
Navigate to the cow management section.
Fill in details like Cow ID, Age, Breed, Date of Ownership, and Number of Offspring.
Save the cow data.
Edit cows:
Select a cow record.
Update the fields and save changes.
Delete cows:
Remove unwanted cow records.
