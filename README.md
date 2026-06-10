# Flask CI/CD Pipeline with GitHub Actions & Docker Hub

## Project Summary

This project establishes a fully automated,  **CI/CD pipeline** using **GitHub Actions** for a containerized **Flask application**. 

Whenever new code is pushed to the repository, the automated workflow triggers immediate execution to handle the entire lifecycle of the application:

1. **Continuous Integration (CI):** Installs Python dependencies and runs automated unit tests with `pytest` to guarantee code stability and quality.
2. **Dockerization:** Builds a high-performance Docker image wrapper containing the updated Flask application environment.
3. **Continuous Deployment (CD):** Authenticates securely, tags the final production build, and automatically pushes the verified container image straight to **Docker Hub** for seamless infrastructure deployment.

---

## Workflow Architecture

```text
[ Developer Push ] ──► [ Run Pytest ] ──► [ Build Docker Image ] ──► [ Push to Docker Hub ]