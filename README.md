MERN Stack Test - README

Project Overview: This project is a web application built using the MERN stack (MongoDB, Express.js, React, Node.js) that implements role-based user management and user dashboards with CRUD operations. It supports three types of users:

Super Admin: Full access to manage workspaces and employees.
Workspace Admin: Manages employees and workspace-related features.
Employee: Can view and edit their personal profile and dashboard.
Features:

Authentication:

Employee Registration: Employees can register with Name, Password, Company, Date of Birth, Department, Mobile, Email, Profile Picture, and Joining Date.
Login: Employees can log in using Name/Email and Password. Workspace Admins and Super Admins can log in with their credentials.
My Profile: Users can view and update their profile details.
User-based Permission Routing: Routes and access control are based on the logged-in user role (Super Admin, Workspace Admin, Employee).
Super Admin Management:

Login & Dashboard: Super Admin can log in and view their workspace.
Workspace Management: The Super Admin can create, edit, or deactivate workspaces (details include Logo, Name, Email, Phone, Address).
Bypass Login: Super Admin can bypass login for any workspace to view workspace data directly.
Profile Management: Super Admin can view and update their profile.
Workspace Admin:

Login & Dashboard: Workspace Admin can log in and see workspace data.
Employee Management: Workspace Admin can view, add/edit, and deactivate employees. Admin can also bypass employee login to see their profile and dashboard.
Profile Management: Workspace Admin can view and update their profile.
Employee Management Module:

Employee CRUD: Workspace Admin can add employees with fields like Name, Email, Phone number, Address, Company name, Company address, Experience.
List/Grid View: Employees can be listed in table or grid view, with filters for Department and Joining Date.
Infinite Scrolling: When using grid view, infinite scrolling is implemented for pagination.
Export Data: Admins can export the employee list in CSV format.
Employee Dashboard:

Profile: Employees can view their profile with details like Name, Email, Phone number, Address, Company name, Company address, and Experience.
Dashboard: Employees can see graphs (Pie, Bar, Line charts) and card layouts with counts and date range filters.
Technologies Used:

Front-End:

React
Redux Toolkit
React Hook Form / Formik
Tailwind CSS
React Charts.js
React Router
TypeScript
Back-End:

Node.js
Express.js
MongoDB
Mongoose (ODM)
JWT (JSON Web Tokens for Authentication)


Installation steps :

Back-End Setup:

Navigate to the backend directory:
bash
Copy code
cd server
Install dependencies:
Copy code
npm install
Create a .env file in the backend folder and add the following:
makefile
Copy code
MONGO_URI=your_mongo_connection_string
PORT=5000
Start the back-end server:
sql
Copy code
npm start
Front-End Setup:

Navigate to the frontend directory:
bash
Copy code
cd client
Install dependencies:
Copy code
npm install
Start the front-end server:
sql
Copy code
npm start
