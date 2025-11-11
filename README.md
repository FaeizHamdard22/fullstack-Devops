# DevOps Full-Stack Project (React + Node.js)

This project is a **full-stack web application** powered by **React (frontend)** and **Node.js (backend)**, fully containerized with **Docker** and orchestrated using **Docker Compose**.  
It also includes **GitHub Actions** for continuous integration and deployment (CI/CD).

---

##  Overview

The main goal of this project is to demonstrate **modern DevOps practices** in a full-stack environment.

**Frontend:** React (developed by another developer)  
**Backend:** Node.js (Express)  
**DevOps Setup:** Docker, Docker Compose, GitHub Actions, and Nginx reverse proxy for deployment.

---

##  Project Structure

fullstack-Devops/
├── .github/
│ └── workflows/
│ └── ci.yml # GitHub Actions workflow file
├── client/ # React frontend
│ ├── public/
│ └── src/
│ ├── components/
│ ├── pages/
│ └── services/
├── server/ # Node.js backend
├── docker-compose.yml # Multi-container setup (frontend, backend, nginx)
├── Dockerfile # Dockerfile for building images
└── README.md

yaml
Copy code

---

##  Technologies Used

- **Frontend:** React.js  
- **Backend:** Node.js (Express)  
- **Proxy / Web Server:** Nginx  
- **Containerization:** Docker  
- **Orchestration:** Docker Compose  
- **CI/CD:** GitHub Actions  
- **Version Control:** Git & GitHub

---

##  Deployment

1. **Clone the Repository**

   ```bash
   git clone https://github.com/FaeizHamdard22/devops-youtube-course-2025.git
   cd devops-youtube-course-2025
Build and Run with Docker Compose

bash
Copy code
docker-compose up --build -d
Access the Application

Frontend → http://localhost:3000

Backend → http://localhost:5000/api

 CI/CD with GitHub Actions
The repository includes a GitHub Actions workflow (.github/workflows/ci.yml) that:

Runs automated tests

Builds Docker images

Pushes images to a container registry

Deploys to a remote server (optional configuration)

 Environment Variables
For local development or CI/CD, make sure to configure a .env file for both backend and frontend services:

bash
Copy code
# Backend .env example
PORT=5000
MONGO_URI=mongodb://localhost:27017/devopsdb
JWT_SECRET=your_secret_key

# Frontend .env example
REACT_APP_API_URL=http://localhost:5000/api
 Author
Faeiz Hamdard

 faeizhamdard48@gmail.com
 GitHub: FaeizHamdard22

🧾 License
This project is licensed under the MIT License — feel free to use and modify.
