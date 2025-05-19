# Valid8 Project

The **Valid8** project consists of a **frontend** and **backend** application, each containerized using Docker. Docker Compose is used to orchestrate both services, making it easier to develop, test, and deploy the application.

---

## 📋 Prerequisites

Make sure you have the following installed on your machine before running the project:

- [Docker](https://www.docker.com/)
- [Docker Compose](https://docs.docker.com/compose/)

---

## ⚙️ Setup Instructions

1. **Clone the repository** to your local machine:

   ```bash
   git clone https://github.com/KHRISTMAE/Valid8-Attendance-Recognition-System.git
   cd Valid8-Attendance-Recognition-System

 ## Create environment variables
      ```bash
       cp .env.example .env
        POSTGRES_USER=admin
        POSTGRES_PASSWORD=admin123
        POSTGRES_DB=valid8db
        
 ## Build and Run the System
 From the project root directory, build and start the containers with:
 
 bash 
- docker-compose up --build

This command will:
- Build the Docker images for backend and frontend
- Start the PostgreSQL database container
- Launch backend and frontend services
- Automatically network all containers for communication

### To stop the running containers:
 bash 
 - docker-compose down

## Access the Application

After successful startup, access the following:

Frontend Dashboard	
- http://localhost:3000
Backend API Documentation
- http://localhost:8000/docs

These ports are configurable via docker-compose.yml or .env files.

##  How It Works
- Backend: FastAPI application serving API endpoints, facial recognition logic, and database interactions.
- Frontend: Web dashboard interface consuming backend APIs for attendance management.
- PostgreSQL: Database container storing all user and attendance data.
- Docker Compose orchestrates all services for simplified local development and deployment.

 

 
  


