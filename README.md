# Arman_Project
For Churchtools
# Project Setup Instructions

## Prerequisites

- Docker
- Docker Compose

## Steps to Run the Application

1. Unzip the project folder to your local machine.
    ```bash
    unzip my_project.zip
    cd my_project
    ```

2. Build and start the Docker containers:

    ```bash
    docker-compose up --scale backend=3
    ```

3. Access the application via HAProxy:

    ```bash
    curl http://localhost:8096/hello
    ```

## Stopping the Application

To stop the application, press `CTRL+C` in the terminal where Docker Compose is running, or run:

    ```bash
    docker-compose down
    ```

## Troubleshooting

- Ensure Docker and Docker Compose are installed and running properly.
- Check for any errors in the terminal output for clues on what might be going wrong.
