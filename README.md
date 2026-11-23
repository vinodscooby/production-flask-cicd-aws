# Production-Ready Flask CI/CD Pipeline on AWS

End-to-end CI/CD pipeline for a Python Flask application using **GitHub Actions**, **Docker**, and **AWS EC2**.

## 🚀 Project Overview

This project demonstrates a complete production-style workflow:

- Source code management with GitHub
- Automated CI pipeline using GitHub Actions
- Containerization with Docker
- Deployment on AWS EC2
- Public access via Security Groups

## 🛠️ Tech Stack

- **Language**: Python 3.12 + Flask
- **CI/CD**: GitHub Actions
- **Containerization**: Docker
- **Cloud**: AWS EC2
- **Testing**: pytest

## 📋 Pipeline Stages

1. Code Checkout
2. Install Dependencies
3. Run Unit Tests
4. Build Docker Image
5. Deploy on AWS EC2

## 🧪 How to Run Locally

```bash
# Clone the repository
git clone https://github.com/vinodscobby/production-flask-cicd-aws.git
cd production-flask-cicd-aws

# Create virtual environment
python -m venv venv
source venv/bin/activate        # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run the application
python -m app.main

Open: http://localhost:8080

# Build the image
docker build -t production-flask-app .

# Run the container
docker run -d -p 8080:8080 --name flask-app production-flask-app

☁️ AWS Deployment
Instance: Ubuntu 22.04 (t2.micro)
Container running on port 8080
Security Group configured to allow public access

production-flask-cicd-aws/
├── app/
│   ├── __init__.py
│   └── main.py
├── tests/
│   └── test_app.py
├── .github/
│   └── workflows/
│       └── cicd.yml
├── Dockerfile
├── requirements.txt
└── README.md


🎯 Key Learnings

.Building CI pipelines with GitHub Actions
.Containerizing Python applications
.Deploying Docker containers on AWS EC2
.Configuring Security Groups for public access
.Troubleshooting real deployment issues

🔗 GitHub Repositoryhttps://github.com/vinodscobby/production-flask-cicd-aws

