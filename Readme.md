## Exp 1 – React Lab Exercise: Understanding React File Structure
## NAME: LIVYA DHARSHINI G
## REG NO: 2305001013
## Aim
To create a basic React application using Vite and understand the purpose of important files and
folders in the React project structure.
## Objectives
1. Create a React project using Vite.
2. Identify important React files and folders.
3. Understand the role of main.jsx , App.jsx , index.html , and package.json .
4. Create and use simple React components.
5. Run and test a React application.
## Program
```
Step 1: Create a React Project

npm create vite@latest student-app
cd student-app
npm install
npm run dev
Select React as the framework and JavaScript as the variant.

Step 2: Understand the File Structure
student-app/
│
├── node_modules/
├── public/
├── src/
│   
├── assets/
│   
├── components/

The index.html file contains the root element where the React application is displayed.
The main.jsx file is the entry point of the React application. It connects React with the HTML root
element and renders the App component.
Create a components folder inside src and add Student.jsx .
│   │   ├── Student.jsx
│   │   ├── Course.jsx
│   │   └── Faculty.jsx
│   │
│   ├── App.css
│   ├── App.jsx
│   ├── index.css
│   └── main.jsx
│
├── index.html
├── package.json
├── package-lock.json
└── vite.config.js

Step 3: Understand index.html

<div id="root"></div>

Step 4: Understand main.jsx

Step 5: Create App.jsx

import './App.css'
function App() {
  return (
    <div className="container">
      <h1>Student Information System</h1>
      <Student />
      <Course />
      <Faculty />
    </div>
  )
}
export default App

Step 6: Create Student.jsx


import '../App.css'
function Student() {
  return (
    <div className="student">
      <h2>Student Details</h2>
      <p>Name: LIVYA DHARSHINI G</p>
      <p>Register Number: 2305001013</p>
      <p>Department: CSE</p>
    </div>
  )
}
export default Student

Step 7: Create Course.jsx

import '../App.css'
function Course() {
  return (
    <div className="student">
      <h2>Course Details</h2>
      <p>Course: AI1067 - Modern Web Application Development</p>
      <p>Semester: VII</p>
      <p>Credits: 3</p>
    </div>
  )
}
export default Course

Step 8: Create Faculty.jsx

import '../App.css'
function Faculty() {
  return (
    <div className="student">
      <h2>Faculty Details</h2>
      <p>Name: Ajith Kumar</p>
      <p>Department: CSE</p>
      <p>Designation: Professor</p>
      <p>College: Saveetha Engineering College</p>
    </div>
  )
}
export default Faculty

Step 9: Import Components in App.jsx

import './App.css'
import Student from './components/Student'
import Course from './components/Course'
import Faculty from './components/Faculty'
function App() {
  return (
    <div className="container">
      <h1>Student Information System</h1>
      <Student />
      <Course />
      <Faculty />
    </div>
  )
}
export default App

Step 10: Add CSS in App.css

.container {
  text-align: center;
  padding: 30px;
}
.student {
  border: 1px solid #ccc;
  padding: 20px;
  margin: 20px auto;
  width: 300px;
}
.student h2 {
  color: blue;
}
.student p {
  color: green;
}
```
## Output
Student Information System

<img width="1254" height="1254" alt="Student Information System Panels" src="https://github.com/user-attachments/assets/db27483a-2b63-4272-96ce-288466a5682f" />



## Result
Thus, a basic React application was successfully created using Vite. The React file structure was
understood, and reusable components were created and displayed successfully.
