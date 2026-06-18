# Containerized-App-Deployment
This DevOps project that demonstrates a complete CI/CD pipeline using Jenkins, Docker, GitHub, and AWS EC2. This project automates the process of building, packaging, and deploying a containerized web application, showcasing a real-world software delivery workflow.The pipeline is designed to reduce manual effort by automatically validating code changes, building Docker images, pushing them to a container registry, and deploying the latest version to an AWS EC2 instance.

## Architecture
Developer
    │
    ▼
 GitHub Repository
    │
    ▼
 Jenkins Pipeline
    │
    ├── Build Docker Image
    ├── Run Validation Checks
    ├── Push Image to Registry
    └── Deploy to AWS EC2
                │
                ▼
        Running Application


Prerequisites

The tools which we use:

Git
Docker
Jenkins
AWS Account
EC2 Instance
Docker Hub Account (or AWS ECR)

# Clone the Repository
git clone https://github.com/your-username/jenkins-cicd-pipeline.git
cd jenkins-cicd-pipeline
# Build the Docker Image
docker build -t sample-app .
# Run the Application
docker run -d -p 80:80 sample-app
# Access the application at:
http://localhost
