# SonarQube Kiaq Lab

## Overview
This project demonstrates static code analysis using SonarQube, SonarScanner CLI, and Jenkins Pipeline.

## Technologies
- Node.js and JavaScript
- SonarQube Community Build
- SonarScanner CLI
- Jenkins Pipeline
- Docker Compose
- Git and GitHub

## Project Structure
- `src/app.js` - Sample JavaScript application
- `sonar-project.properties` - SonarQube project configuration
- `Jenkinsfile` - Jenkins pipeline
- `compose.yaml` - SonarQube container configuration
- `screenshots/` - Assessment evidence

## Start SonarQube
Run:
`sudo docker compose up -d`

Open http://localhost:9000.

## Run the sample application
Run:
`node src/app.js`

## Run SonarQube analysis
Configure `SONAR_TOKEN` securely in your terminal and run:
`sonar-scanner`

Never commit tokens or passwords.

## Jenkins Integration
The Jenkins pipeline checks out the repository and runs SonarScanner against the configured SonarQube server.

## Initial Analysis
The initial scan completed successfully. The dashboard showed a passed Quality Gate and zero issues at the time of analysis.

## Assessment Submission
- SonarQube dashboard screenshot
- SonarScanner configuration
- Jenkins pipeline screenshot
- Quality Gate result
- Analysis report
- GitHub repository URL
- README documentation

## Security
Do not commit credentials, private keys, `.env` files, or tokens.
