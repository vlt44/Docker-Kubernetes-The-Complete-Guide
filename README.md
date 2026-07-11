# Docker-Kubernetes-The-Complete-Guide

This repository contains my coursework, notes, exercises, and projects completed while studying:

- Course: [Docker and Kubernetes: The Complete Guide](https://www.udemy.com/share/101WjM3@e9IN8-R3buEAdALNOvZQURCtCAvgY1qBnW_Co5YNkmAni67O4-xYYcX7ym8SFexpFg==/)
- Instructor: Stephen Grider
- Platform: Udemy

The course covers containerization, orchestration, CI/CD pipelines, cloud deployments, and production-ready application workflows using Docker and Kubernetes.

### Technologies

- Docker
- Docker Compose
- Kubernetes
- Travis CI
- GitHub
- AWS
- Google Cloud Platform
- Node.js
- React
- Redis
- PostgreSQL
- Skaffold

## Projects

### Simple Web Application

- Docker Port Forwarding

- Building and Running a Docker Container
  ![build logs](./simple-web/img-build.png)

- Docker Port Mapping Syntax: `docker run -p 8080:8080`

- Inspecting and Accessing a Running Container
  ![build logs](./simple-web/img-shell.png)

- Create new database
  ![CreateDB](/simple-web/img-createDB.png)

<br />

### Visits Application

Objectives: Docker Compose with Multiple Local Containers

- docker containers
- images
- docker cli
- docker compose

<br />

![projectArchitecture](./visits/img-projectArchitecture.png)
![allContainersRunning](./visits/img-allContainerRunning.png)
![browser](./visits/img-browser.png)

#### Docker Compose

Launch Containers in Background

```bash
docker-compose up -d
```

Stop Containers

```bash
docker-compose down
```

Container Exit Status Codes

| Status Code    | Meaning                                     |
| -------------- | ------------------------------------------- |
| `0`            | Container exited successfully.              |
| `1, 2, 3, ...` | Container exited because an error occurred. |

Docker Restart Policies

| Policy           | Description                                                                                                         |
| ---------------- | ------------------------------------------------------------------------------------------------------------------- |
| `no`             | Never restart the container if it stops or crashes. _(Default)_                                                     |
| `always`         | Always attempt to restart the container whenever it stops, regardless of the reason.                                |
| `on-failure`     | Restart the container only if it exits with a non-zero (error) status code.                                         |
| `unless-stopped` | Always restart the container unless it was explicitly stopped by the user (`docker stop` or `docker-compose down`). |

<br/>

### Production Grade Workflow Application

![workflow](./flow/img-workflow.png)
![workflowDetails](./flow/img-workflowDetails.png)

<br/>

#### Dev Enviroment

![successfulDevBuild](./flow/img-successfulDevBuild.png)
![successfulDevStartup](./flow/img-successfulDevStartup.png)
![SetupVolumn](./flow/img-setupVolumn.png)
![SuccessfulVolumnMount](./flow/img-successfulVolumnMount.png)

<br/>

#### Test Enviroment

Live Updating Solution 1
![liveUpdatingTests](./flow/img-liveUpdatingTests.png)

Live Updating Solution 2
![testContainerAndProcesses](./flow/img-testContainerAndProcesses.png)

#### Prod Environment

![multistepBuild](./flow/img-multistepBuild.png)

**testing**
