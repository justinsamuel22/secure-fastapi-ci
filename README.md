[![CI](https://github.com/justinsamuel22/secure-fastapi-ci/actions/workflows/ci.yaml/badge.svg)](https://github.com/justinsamuel22/secure-fastapi-ci/actions/workflows/ci.yaml)
[![Known Vulnerabilities](https://snyk.io/test/github/justinsamuel22/secure-fastapi-ci/badge.svg)](https://snyk.io/test/github/justinsamuel22/secure-fastapi-ci)

# Secure FastAPI CI Demo


## Overview
This is a minimal Python API used to demonstrate CI testing and security scanning of dependencies using GitHub Actions and Snyk. 

## Features
- Simple FastAPI Rest API with health and version endpoints
- Automated tests using pytest
- GitHub Actions CI pipeline
- Snyk dependency vulnerability scanning as a security gate

## CI & Security
Whenever a push or pull request occurs to the `main` branch:
1. A runner installs required Python dependencies
2. Automated tests will run
3. Snyk scans dependencies for any known vulnerabilities
4. The pipeline will fail if the initial test fails or if high-severity vulnerabilities are detected

## Endpoints
- `GET /health` - service health check
- `GET /version` - application version check

## Tech Stack
- Python 3
- FastAPI
- pytest
- GitHub Actions
- Snyk

## Purpose
This project demonstrates a simplified DevSecOps workflow:
Develop -> Test -> Commit -> CI -> Security Gate -> Push
