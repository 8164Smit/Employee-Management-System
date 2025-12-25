📌 Employee Management System – Project Description
1️⃣ Project Overview

This project is a Employee Management System developed using React JS.

It performs CRUD operations (Create, Read, Update, Delete) on employee data.

The application stores data in the browser’s LocalStorage, so no backend or database is required.

2️⃣ Technologies Used

React JS – For building user interface components.

React Router DOM – For navigation between pages.

Vite – For fast React project setup and development.

CSS – For styling, centering layout, and glowing UI effects.

LocalStorage – For persistent data storage in the browser.

3️⃣ Application Structure

The application consists of multiple pages:

Home Page – Displays project overview.

Add Employee Page – Allows adding new employee details.

Employee List Page – Displays all employees in a tabular format.

Edit Employee Page – Allows updating employee details.

Delete Functionality – Removes employee records.

Routing is handled using react-router-dom.

4️⃣ Add Employee Functionality

A form is provided to enter:

Name

Email

Role

Salary

Employee Photo (file upload)

The image is converted into a Base64 string using FileReader and stored in LocalStorage.

On form submission:

A unique id is generated using Date.now().

The employee object is added to LocalStorage.

User is redirected to the Employee List page.

5️⃣ View Employee List

All employee data is fetched from LocalStorage using useEffect.

Data is displayed in a table layout with columns:

Photo

Name

Email

Role

Salary

Actions

Employee images are displayed using <img> tags.

If no employees exist, a message “No Employees Found” is shown.

6️⃣ Edit Employee Functionality

Each employee row has an Edit button.

Clicking Edit:

Navigates to /edit/:id using useNavigate.

Employee data is fetched using useParams.

The form is pre-filled with existing employee details.

On update:

The selected employee is updated in LocalStorage.

User is redirected back to the Employee List page.

7️⃣ Delete Employee Functionality

Each employee row has a Delete button.

On clicking Delete:

A confirmation popup is shown.

The selected employee is removed using filter().

LocalStorage is updated instantly.

The UI updates without page refresh.

8️⃣ State Management

useState is used to manage:

Form inputs

Employee list

useEffect is used to:

Fetch employee data from LocalStorage when the component loads.

9️⃣ UI & Styling Features

All pages are center-aligned for better readability.

Table layout is used for clean data presentation.

Employee photos are styled with rounded borders.

Buttons have hover effects for better user interaction.

Dark theme with glowing highlights is used for a modern UI.

🔟 Data Persistence

Employee data remains saved even after page refresh.

This is achieved using LocalStorage, eliminating the need for backend APIs.

✅ Conclusion

This project demonstrates a complete React CRUD application.

It effectively uses React Hooks, Routing, and LocalStorage.

The application is scalable and can be extended with:

Backend integration

Authentication

Search and filter options

<img width="1920" height="1030" alt="First" src="https://github.com/user-attachments/assets/ca4025b4-6b92-4f7e-b549-da48cda064b5" />

<img width="1920" height="1030" alt="Second" src="https://github.com/user-attachments/assets/a319532a-0b3b-4ac9-bc5a-a2e27dae0b3c" />

<img width="1920" height="1030" alt="Third" src="https://github.com/user-attachments/assets/e83db2d4-cd2f-4879-b301-6e1676243b5d" />
