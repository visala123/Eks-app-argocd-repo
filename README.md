# Streamlining Kubernetes Deployments: CI/CD with GitHub Actions and Helm for EKS
## Architecture Diagram
![Architecture](https://github.com/visala123/Eks-app-repo/blob/cd5d9c4b141a4f05f88dc684094c650c6089ccd1/Architecture.png)

## Values.yaml
update the values.yaml repository: XXXXXXXXXXXX.dkr.ecr.ap-northeast-2.amazonaws.com/eks-app-repo   #ECR registry URI 

## Sonar Scanner

SonarScanner Setup: Create an organization in sonarcloud

Open the browser and navigate to www.sonarcloud.io, click the "+" at the top right corner and create a new organization -> create one manually

name: github-actions-cicd

key: github-actions-cicd -> Create

Click analyze new project

Organization: github-actions-cicd

display name: github-actions

Project key: github-actions -> Next

The new code for this project will be based on: Previous version=true

-> Create project

Copy the sonar token and paste it in notepad, click on information on the left, copy the values of organization, project key and create secrets in Github settings

SonarQube Scan: Analyzes code quality, test coverage, style violations, and sends the results to a configured SonarQube instance.

Secrets used:

SONAR_URL, SONAR_TOKEN, SONAR_ORGANIZATION, SONAR_PROJECT_KEY


