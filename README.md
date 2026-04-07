# Job Portal UI (React.js)

A modern Job Portal user interface built with **React.js**, styled using **CSS** and **Bootstrap**, and enhanced with **JavaScript logic**.  
This application allows users to **fetch all jobs**, **create new job postings**, and **manage job contacts** seamlessly.  

---

## 🚀 Features
- **Job Listings**: Fetch and display all available jobs.
- **Create Job**: Add new job postings with relevant details.
- **Contacts Management**: Create and manage job-related contacts.
- **Responsive UI**: Built with Bootstrap grid system and custom CSS.
- **Modern Stack**: React.js + Axios + Material UI + Bootstrap.

---

## 🛠 Tech Stack
- **Frontend**: React.js (Hooks, Functional Components)
- **Styling**: CSS, Bootstrap (`bootstrap/dist/css/bootstrap.min.css`)
- **UI Library**: Material UI (`@mui/material`, `@mui/icons-material`)
- **HTTP Client**: Axios
- **JavaScript**: ES6+ features integrated with React
- **Tooling**: npm, VS Code, json-server

---

## 📂 Project Structure
```
jobportal-react-1/
  ├── public/
  ├── src/
  │    ├── components/   # Reusable UI components
  │    ├── pages/        # Job listing, create job, contacts
  │    ├── styles/       # Custom CSS files
  │    ├── App.js        # Main app entry
  │    └── index.js      # React DOM render
  ├── db.json            # Mock backend data for json-server
  ├── package.json
  └── README.md
```

## ⚡ Getting Started

### Clone the Repository
```bash
git clone https://github.com/sugganabalaji/jobportal-react-1.git
cd jobportal-react-1
```
## Installation & Setup

### 1. Create a new React app (already scaffolded in repo, but for reference)
npx create-react-app jobportal-react-1

### 2. Navigate into the project
cd jobportal-react-1

### 3. Start the React development server
npm start

## Backend (Mock API with json-server)

### 4. Install json-server globally
npm install -g json-server

### 5. Run json-server with db.json on port 8000
json-server --watch db.json --port 8000

## Final Steps

### 6. Install dependencies (if not already installed)
npm install

### 7. Start the React app again
npm start

## 🌐 Access the Application
Once the server starts, open your browser and go to:
#### 👉 http://localhost:3000/

Mock backend runs at:
#### 👉 http://localhost:8000/posts

## 🔗 API Integration
This UI is designed to connect with a backend (e.g., Spring Boot REST API or json-server).
Update API endpoints in your Axios service files
```Javascript
import axios from "axios";

const API = axios.create({ baseURL: "http://localhost:8000" });

export const fetchJobs = () => API.get("/jobs");
export const createJob = (jobData) => API.post("/jobs", jobData);
export const createContact = (contactData) => API.post("/contacts", contactData);
```
### Spring Boot Rest API also needs to up and run in your locally.
- Project `spring-boot-rest` is Backend integration project for this application.
- Used `Maven`, `Spring Boot`, `Spring Data JPA` and `PostGreSQL`.
- Git Repo link provided below
```bash
  https://github.com/sugganabalaji/spring-boot-rest.git
```
- URL will look like `http://localhost:8080/`
- PostGreSQL install in your local
- Create a schema as `Dev`
- Execute `GET Api - http://localhost:8080/loadData` from Postman or browser, to load sample data to PostGre DB.
- In PostGreSQL Table `JobPost` Automatically created
- Used Intellij IDEA to build and run the Application
  
## 👨‍💻 Author
Balaji Suggana

Senior Software Engineer | Modernizing Java/Spring/Maven portfolio ready projects
```
This README now includes:  
- ✅ Your **GitHub clone URL** ('https://github.com/sugganabalaji/jobportal-react-1.git')  
- ✅ Full setup steps ('npx create-react-app', 'json-server', 'npm install', 'npm start')  
- ✅ Access instructions for **http://localhost:3000** and **http://localhost:8000**  
```
