# Student Information Web Application

## Project Overview

This project is a simple web application designed to manage student information. It consists of two main pages:
- **Add Student Page**: Allows users to input and submit new student information.
- **View Students Page**: Displays all the student information stored in the database.

## Project Goal

The primary goal of this project is to deploy the web application using Docker and Docker Compose, ensuring that the frontend, API, and database services run seamlessly within Docker containers.

## Technologies Used

- **Frontend**: Flask
- **Backend API**: FastAPI
- **Database**: PostgreSQL (using an existing Docker image)
- **Containerization**: Docker, Docker Compose

## Running the Project

Follow these steps to build and run the Dockerized web application on your local machine.

### Prerequisites

- Ensure Docker and Docker Compose are installed and running on your machine.

### Step-by-Step Tutorial

#### Step 1: Clone the Repository

First, clone the project repository to your local machine using Git.

```sh
git clone <repository-url>
cd <repository-directory>

#### Step 3: Run the Containers

After building the images, use Docker Compose to start the containers. The `-d` flag runs the containers in detached mode, allowing you to continue using the terminal.

```sh
docker-compose up -d

#### Step 4: Verify the Containers

Ensure that all containers are running correctly by listing the active containers.

```sh
docker ps

You should see three containers running: `database`, `api-run`, and `web-app`.

#### Step 5: Access the Application

Open your web browser and navigate to the following URLs to access the frontend of the web application:

```sh
http://localhost:8090/add
http://localhost:8090/all

You should see the "Student Information Form" page where you can add new student information.



