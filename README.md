Instructions for Building and Running Software and Unit Tests
●	Build Instructions:
1. Ensure that you have Docker installed on your system.
2. Navigate to the project directory.
3. Build the Docker image using the provided Dockerfile:
   docker build -t phonebook-app .

●	Running Software:
1. Run the Docker container:
   docker run -p 8000:8000 phonebook-app
2. The FastAPI application will be accessible at http://localhost:8000.

●	Running Unit Tests:
1. Ensure that the Docker container is running.
2. Open a new terminal.
3. Run the following command to execute the unit tests:
   docker exec -it CONTAINER_ID pytest testmain.py
