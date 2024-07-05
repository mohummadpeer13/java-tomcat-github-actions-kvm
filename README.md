# java-tomcat-github-actions-kvm
Java Spring Boot project with Postgres DB - CICD Github Actions and deploy on my own local server (OS ubuntu 22.04 - Kvm VM - Docker)

Docker container for Java based on: Tomcat, PostgreSQL

# Build Spring Boot Project
./mvnw clean package -DskipTests

# Build Docker Postgres and Tomcat
docker-compose up -d

# Re-build image
docker-compose up --build

# Run
http://localhost:8080

# Enter to Docker container.
docker exec -it tomcat bash

# Debug
Listen to port 61000 for debugging

