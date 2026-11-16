# Project Architecture

## Overview

The project uses a DevSecOps architecture to automate and secure application deployment.

## Workflow

1. Developer writes code on Windows using VS Code.
2. Code is pushed to GitHub.
3. Jenkins running on a VMware Linux VM retrieves the code.
4. Jenkins executes CI/CD pipeline stages.
5. Terraform manages Azure infrastructure.
6. Checkov scans Terraform configurations.
7. Docker builds application images.
8. Trivy scans container images.
9. Kubernetes runs the application.

## Main Components

- GitHub: source code management.
- Jenkins: CI/CD automation.
- Terraform: Infrastructure as Code.
- Azure: cloud infrastructure.
- Docker: containerization.
- Kubernetes: container orchestration.
- Checkov and Trivy: security scanning.