# Container Observability Report

## Application Logs
- **Log Evidence (404 Error):**
172.17.0.1 - - [07/Oct/2026:01:42:47 +0000] "GET /hidden-admin-page HTTP/1.1" 404 153 "-" "curl/8.5.0" "-"

### Explanation
Application logs are very important, because they provide a detailed record of every request and error inside the container. They also allow engineers to trace problems back to specific events, making troubleshooting faster and more accurate. Logs act like a security camera, showing what happened, when it happened, and how the system responded.

## Real‑Time Container Metrics
- **Memory Usage:** 2.828 MiB / 1.859 GiB (≈0.15%) 
- **CPU Usage:** ~0.00%  

### Explanation
Real‑time metrics are important, because they show how efficiently the container is using system resources. While logs reveal what happened, metrics prove whether the application is running within safe limits. Monitoring CPU and memory ensures the container won’t overload the host during heavy traffic.
