## Technical Project Specification: Distributed Monolithic Cinema Application

### Overview
The aim of the project is to create a distributed monolithic cinema application using Django for front-end, Django Rest Framework (DRF) for the back-end, and Postgres for the database. Each part of the application will run in separate Docker containers, and they will be orchestrated using Docker Compose.

The application will provide functionality to fetch and display a list of all movies, as well as detailed information about each movie.

### Front-end Service

1. Develop a Django application that will serve as the front-end service.
2. Use Django templates to create user interfaces that display a list of all movies and detailed movie information.
3. Implement HTTP requests to the back-end service using Python libraries such as requests or Django's built-in functions.
4. The front-end service will be running on a separate Docker container.

### Back-end Service

1. Develop a separate Django application that will serve as the back-end service.
2. Implement Django Rest Framework to create API endpoints for fetching all movies and detailed information about a particular movie.
3. The back-end service will interact with the Postgres database to fetch and store movie data.
4. The back-end service will be running on a separate Docker container.

### Database

1. Set up a Postgres database to store the movie data.
2. The database will be running on a separate Docker container.

### Docker Compose

1. Use Docker Compose to manage and orchestrate the three Docker containers.
2. Ensure all containers can communicate effectively with each other.
3. Configure Docker Compose to automatically start all services in the correct order (database, back-end, front-end).

### Requirements

1. Ensure that the application can handle and gracefully recover from potential errors (e.g., failed requests, server errors).
2. The application should be easy to start with a single Docker Compose command.
3. Implement proper logging for debugging and monitoring purposes.
4. Follow good software development practices: organize your code well, comment your code where necessary, and follow the Python/Django naming conventions and style guides.

Remember, this is a learning experience. Be sure to reach out for help when you encounter challenges. Happy coding!