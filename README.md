# Containerized-App-Deployment
This DevOps project that demonstrates a complete CI/CD pipeline using Jenkins, Docker, GitHub, and AWS EC2. This project automates the process of building, packaging, and deploying a containerized web application, showcasing a real-world software delivery workflow. The pipeline is designed to reduce manual effort by automatically validating code changes, building Docker images, pushing them to a container registry, and deploying the latest version to an AWS EC2 instance.

## Architecture
                                          
              Developer
                   │
                   ▼
          Flask Application
                   │
                   ▼
             Dockerfile
                   │
                   ▼
        Docker Image Creation
                   │
                   ▼
          Docker Container
                   │
                   ▼
        Application on Port 5000
                   │
                   ▼
              Web BrowserPrerequisites                                    



# Clone the Repository
git clone https://github.com/VarshaRajashekar/Containerized-App-Deployment.git
cd jenkins-cicd-pipeline

# Build the Docker Image
docker build -t sample-app .

# Run the Application
docker run -d -p 80:80 sample-app

Verification Commands

Check Docker Version

docker --version

List Images

docker images

List Running Containers

docker ps

List All Containers

docker ps -a

View Container Logs

docker logs flask-container

Execute Commands Inside the Container

docker exec -it flask-container bash
