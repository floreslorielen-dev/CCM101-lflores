# Multi-Tier Architecture

## Two-Tier Architecture
A two-tier architecture is a way of organizing an application into two main layers that work together: the Web/Application Tier and the Database Tier.

### The Web/Application Tier
This is the “front end” where users interact. It handles requests from a browser, processes them, and shows the user interface. it is the Nextcloud container acts as the web/application tier.

### The Database Tier
This is the “back end” where data is stored. It keeps user accounts, file metadata, and other important information safe and available. In this lab, the MariaDB container is the database tier.

### Why separate them?
Separating them makes the system more secure, easier to maintain, and scalable. For example, we can upgrade the database without touching the web app, or restart the web app without losing stored data. It also prevents one failure from crashing the entire system.
