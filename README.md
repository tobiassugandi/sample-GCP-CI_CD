# Sample GCP CI/CD Project

This repository demonstrates a simple CI/CD pipeline setup using Google Cloud Platform (GCP) services. It includes a simple Go application, Docker configuration, and Kubernetes deployment files for both development and production environments.

## Project Structure

```
.
├── Dockerfile
├── cloudbuild-dev.yaml
├── cloudbuild.yaml
├── main.go
├── dev
│   └── deployment.yaml
└── prod
    └── deployment.yaml
```

## Files Description

- **Dockerfile**: Defines the steps to build the Docker image for the Go application.
- **cloudbuild-dev.yaml**: Google Cloud Build configuration for the development environment.
- **cloudbuild.yaml**: Main Google Cloud Build configuration file.
- **main.go**: Source code of the Go application. The application is a simple web server that generates and serves images. It has two endpoints:
  - `/blue`: Serves a blue-colored image.
  - `/red`: Serves a red-colored image.
- **dev/deployment.yaml**: Kubernetes deployment configuration for the development environment.
- **prod/deployment.yaml**: Kubernetes deployment configuration for the production environment.
