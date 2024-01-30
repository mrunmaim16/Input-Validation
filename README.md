Instructions for Building and Running Software and Unit Tests
●	Build Instructions:
Ensure that you have Docker installed on your system.
Navigate to the project directory.
Build the Docker image using the provided Dockerfile:
docker build -t phonebook-app .

●	Running Software:
Run the Docker container:
docker run -p 8000:8000 phonebook-app
The FastAPI application will be accessible at http://localhost:8000.

●	Running Unit Tests:
Ensure that the Docker container is running.
Open a new terminal.
Run the following command to execute the unit tests:
docker exec -it CONTAINER_ID pytest testmain.py
