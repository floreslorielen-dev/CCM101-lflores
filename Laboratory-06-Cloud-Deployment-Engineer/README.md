# Laboratory 06 – Cloud Deployment Engineer

## Mission Overview
In this laboratory, we implemented a multi-container private cloud storage system that utilizes Nextcloud and MariaDB, orchestrated through Docker Compose. This setup exemplifies the concept of Infrastructure as Code (IaC) by representing the entire stack configuration in a YAML file, thereby facilitating reproducibility and version control in the deployment process.

## Objectives
- Explain multi-tier application architecture
- Understand and write a docker-compose.yml file
- Deploy a multi-container application using Docker Compose
- Document Infrastructure as Code principles
- Expand the Cloud Computing Portfolio on GitHub

## Commands Executed
```bash
mkdir nextcloud-deployment
cd nextcloud-deployment
nano docker-compose.yml
docker-compose up -d
docker-compose ps
docker-compose down
