# FastAPI with Domain Driven Design & CQRS

This project demonstrates the use of Domain Driven Design (DDD) and Command Query Responsibility Segregation (CQRS) principles in building applications with FastAPI. It's structured to provide a clear separation of concerns, modular design, and scalable architecture.

## Features
- **FastAPI Integration:** Utilizes FastAPI for building efficient and scalable web APIs.
- **Domain Driven Design:** Implements DDD to focus on the core domain logic.
- **CQRS Pattern:** Separates read and write operations for improved performance and scalability.
- **Docker Support:** Includes a Dockerfile for easy deployment and containerization.
- **Comprehensive Test Suite:** Ensures code quality and reliability with unit and integration tests.

## Project Structure
The project is organized into multiple directories, each serving a specific purpose in the application architecture:

- `src/`: Source code of the application.
  - `apps/`: Contains the main applications or services.
    - `backoffice/`: A backoffice application module.
    - `photostore/`: A photo storage service module.
  - `contexts/`: Domain contexts for DDD.
    - `backoffice/`: Context for backoffice domain.
    - `photostore/`: Context for photo storage domain.
  - `shared/`: Shared infrastructure and domain logic.
  - `utils/`: Utility scripts and helpers.
- `tests/`: Contains all unit and integration tests.
- `Dockerfile`: Docker configuration file.
- `LICENSE`: Project license.
- `Makefile`: Simplifies command execution.
- `main.py`: Entry point of the application.
- `requirements.txt`: Lists all the Python dependencies.

## Getting Started
To get started with this project, clone the repository and install the dependencies:

```bash
git clone [repository-url]
cd [project-name]
pip install -r requirements.txt
```

## Running the Application
You can start the application using the following command:

```bash
python main.py
```

For Docker users, you can build and run the container using the provided Dockerfile.

## Testing
Run the tests using the following command:

```bash
pytest
```