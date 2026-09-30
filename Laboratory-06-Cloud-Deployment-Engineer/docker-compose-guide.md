# Docker Compose Guide

## What does the `services` block do?
The `services` block defines the different containers that make up the application. In this deployment, there are two services. The first service is called database, and it runs MariaDB. This container stores user accounts, file metadata, and configuration settings. The second service is called app, and it runs Nextcloud. This container provides the web interface where users can log in, upload files, and interact with the cloud system.

## How did the Nextcloud app container know how to find the database container?
The Nextcloud container knows how to connect to the MariaDB container because of the environment variable MYSQL_HOST=database. Docker Compose automatically creates a private network where services can communicate using their names. Since the database service is named database, Nextcloud can reach it directly without needing an IP address.

## Difference between `docker run` and `docker-compose up -d`
- `docker run` it launches a single container with specific options. You used this earlier for standalone deployments.
- `docker-compose up -d` it launches multiple containers at once based on the YAML file. This is Infrastructure as Code (IaC), meaning the entire stack is defined in one file and deployed consistently with a single command.
