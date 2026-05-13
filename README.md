## DevOps Setup



This project is containerized using Docker and Docker Compose. The application has three services:



- `frontend`: Builds the React + Vite application and serves the static files with Nginx.

- `backend`: Builds and runs the .NET API using a multi-stage Docker build.

- `nginx`: Acts as the reverse proxy. It routes frontend traffic to the frontend container and `/api/` traffic to the backend container.



### Running locally



From the root of the repository, run:



```bash

docker compose up --build -d
