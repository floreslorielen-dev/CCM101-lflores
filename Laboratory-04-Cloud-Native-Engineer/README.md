# Laboratory 04 – Cloud-Native Engineer

## Mission Overview
This laboratory introduces the shift from traditional virtualization to containerization. Using KillerCoda, I learned how to pull, run, manage, and remove Docker containers by deploying an Nginx web server in just a few seconds.

## Objectives
- Differentiate between Virtual Machines (VMs) and Containers
- Access a Docker-enabled cloud environment using KillerCoda
- Execute fundamental Docker CLI commands
- Pull, run, manage, and terminate a containerized application (Nginx)
- Create professional technical documentation using Markdown
- Continue developing a well-organized GitHub Cloud Computing Portfolio

## Docker Commands Executed
- `docker --version`
- `docker info`
- `docker pull nginx`
- `docker run -d -p 8080:80 --name my-nginx nginx`
- `curl http://localhost:8080`
- `docker ps`
- `docker stop my-nginx`
- `docker ps -a`
- `docker rm my-nginx`

## Skills Learned
- Understanding the architectural differences between Virtual Machines and Containers
- Using the Docker CLI to manage the full container lifecycle
- Port mapping and verifying containerized web services
- Writing clear and organized technical documentation in Markdown
- Maintaining a professional GitHub portfolio structure

## Challenges Encountered
One of the main challenges I faced was distinguishing the differences between Virtual Machines and Containers, especially understanding how isolation works at the hardware versus process level. I also initially struggled with remembering the correct syntax for port mapping (-p 8080:80) when deploying the Nginx container. Another difficulty was managing the container lifecycle, since stopping a container does not remove it, and I had to learn the difference between docker stop and docker rm.
