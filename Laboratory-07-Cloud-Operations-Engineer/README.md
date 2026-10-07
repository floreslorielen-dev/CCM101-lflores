# Laboratory 07 – Cloud Operations Engineer

## Mission Overview
In This Laboratory, we focused on observability and monitoring in a cloud environment.  
we deployed a containerized Nginx web server, generated traffic, and analyzed system health using logs and metrics. The goal was to prove that both the host system and containers can be monitored effectively to ensure reliability.

---

## Objectives
- Establish a baseline for host CPU, memory, and disk.
- Deploy a containerized web server and simulate traffic.
- Capture application logs and identify HTTP errors.
- Monitor real-time container metrics.

---

## Monitoring Commands Executed
- `free -h`
- `df -h`  
- `top`  
- `docker run -d -p 8080:80 --name client-website nginx`  
- `curl http://localhost:8080`   
- `curl http://localhost:8080/hidden-admin-page`   
- `docker logs client-website`   
- `docker stats`
---

## Skills Learned
- Using Linux CLI tools for baseline monitoring  
- Deploying and testing Docker containers  
- Analyzing logs for troubleshooting  
- Observing container resource usage  
- Writing structured technical documentation in Markdown  
- Practicing Site Reliability Engineering principles
