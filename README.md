# SonarQube GitHub Actions Demo

## Objective

This project demonstrates the integration of SonarQube
with GitHub Actions for automated code quality analysis.

## Technologies

- Python
- PyTest
- Coverage.py
- SonarQube
- Docker
- AWS EC2
- GitHub Actions

## Architecture

GitHub Repository
        |
        v
GitHub Actions
        |
        v
SonarQube Scanner
        |
        v
AWS EC2
        |
        v
SonarQube Dashboard

## Project Structure

src/
    calculator.py

tests/
    test_calculator.py

.github/
    workflows/
        sonarqube.yml

sonar-project.properties
requirements.txt

## CI/CD Workflow

The GitHub Actions workflow performs the following:

1. Checks out the source code.
2. Sets up Python.
3. Installs project dependencies.
4. Runs unit tests.
5. Generates the coverage report.
6. Runs SonarQube analysis.
7. Sends the analysis results to the SonarQube server.

## SonarQube Metrics

The project is analyzed for:

- Bugs
- Vulnerabilities
- Code Smells
- Code Coverage
- Duplications
- Reliability
- Security
- Maintainability

## Infrastructure

SonarQube is hosted on an AWS EC2 instance
using Docker.

## Result

The SonarQube dashboard displays the code quality
analysis after every push to the main branch.