# Jenkins 101

Welcome to **Jenkins 101** — a beginner-friendly repository dedicated to helping you learn the fundamentals of DevOps using Jenkins. This project is designed as a hands-on introduction to setting up, running, and understanding Jenkins, with everything containerized for simplicity.

## 🚀 About This Project

This repository provides:
- A simple Docker-based setup for Jenkins
- Step-by-step instructions to get Jenkins up and running locally
- Basic usage examples for pipelines and automation
- Guidance for extending Jenkins for your own DevOps projects

## 🐳 Getting Started

### Prerequisites

- [Docker](https://www.docker.com/get-started) installed on your machine

### Quick Start

1. **Clone the repository:**
   ```bash
   git clone https://github.com/clintoo/jenkins-101.git
   cd jenkins-101
   ```

2. **Build and run Jenkins with Docker:**
   ```bash
   docker build -t my-jenkins .
   docker run -p 8080:8080 -p 50000:50000 my-jenkins
   ```

3. **Access Jenkins:**
   - Open your browser and go to [http://localhost:8080](http://localhost:8080)
   - Follow the initial setup instructions. The admin password can usually be found by running:
     ```bash
     docker exec <container_id> cat /var/jenkins_home/secrets/initialAdminPassword
     ```

### Dockerfile Overview

This repository contains a Dockerfile that:
- Uses the official Jenkins LTS image as its base
- Can be customized to include your own plugins, jobs, and configuration

## 📚 Learning Objectives

- Understand what Jenkins is and why it is used in DevOps
- Learn to install and run Jenkins locally using Docker
- Explore Jenkins pipelines and basic automation tasks
- Discover how to customize Jenkins for your own development workflows

## 📝 Useful Resources

- [Jenkins Documentation](https://www.jenkins.io/doc/)
- [Jenkins Pipeline Tutorial](https://www.jenkins.io/doc/pipeline/tour/getting-started/)
- [Docker Documentation](https://docs.docker.com/)

## 🤝 Contributing

Contributions are welcome! Please open an issue or submit a pull request if you have improvements, questions, or suggestions.

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
