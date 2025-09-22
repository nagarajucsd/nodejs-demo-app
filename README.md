# Node.js CI/CD Demo App

## Overview
This project demonstrates a CI/CD pipeline using GitHub Actions and DockerHub. It automates build, test, and deployment of a Node.js web application.

## Workflow
- Trigger: Push to `main` branch
- Steps:
  1. Checkout code
  2. Install dependencies
  3. Run tests
  4. Build Docker image
  5. Push Docker image to DockerHub

## Files
- `index.js` → Node.js web app
- `package.json` → Node.js dependencies
- `Dockerfile` → Docker image build instructions
- `.github/workflows/main.yml` → CI/CD workflow

## Run Locally
```bash
docker build -t YOUR_DOCKER_USERNAME/nodejs-demo-app:latest .
docker run -p 3000:3000 YOUR_DOCKER_USERNAME/nodejs-demo-app:latest
