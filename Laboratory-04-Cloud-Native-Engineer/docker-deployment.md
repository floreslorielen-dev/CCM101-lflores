# Docker Deployment – Container Lifecycle

1. `docker ps`  
   Displays all currently running containers

2. `docker stop my-nginx`  
   Stops the running Nginx container, ending its process without deleting it.

3. `docker ps -a`  
   Shows all containers (running and stopped) so we can confirm the container is no longer running.

4. `docker rm my-nginx`  
   Permanently deletes the stopped container from the system.
