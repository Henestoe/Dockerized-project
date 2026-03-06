# Dockerized VProfile Application

This project demonstrates how to containerize a multi-tier web application using Docker and Docker Compose.

The application stack includes:

- Nginx (Web Server)
- Tomcat (Application Server)
- MySQL (Database)
- Memcached (Caching Layer)
- RabbitMQ (Message Queue)

All services are containerized and orchestrated using Docker Compose.

---

## Project Architecture

The system consists of the following containers:

1. **Nginx**
   - Acts as the web server and reverse proxy.

2. **Tomcat**
   - Runs the Java web application.

3. **MySQL**
   - Stores application data.

4. **Memcached**
   - Provides caching to improve performance.

5. **RabbitMQ**
   - Handles messaging between application components.

---

## Project Structure

Dockerized-project

│
├── Docker-files
│ ├── app
│ │ └── Dockerfile
│ ├── db
│ │ └── Dockerfile
│ └── web
│ └── Dockerfile
│
├── docker-compose.yml
├── Vagrantfile
└── README.md


---

## Prerequisites

Make sure the following are installed:

- Docker
- Docker Compose
- Git
- Vagrant (optional if using VM)

---

## How to Run the Project

### Step 1: Clone the repository
git clone https://github.com/Henestoe/Dockerized-project.git

cd Dockerized-project

### Step 2: Build the images
docker compose build

### Step 3: Start the containers
docker compose up -d

### Step 4: Verify running containers
docker compose ps

## Useful Docker Commands

Check running containers: docker ps
View logs: docker logs <Container-name>
Stop containers: docker compose down

## Author
Adegbola Adeniyi (Henex)
