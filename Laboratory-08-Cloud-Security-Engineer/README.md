# Laboratory 08 – Cloud Security Engineer

## Mission Overview
In this mission, I stepped into the role of a Cloud Security Engineer to secure a vulnerable Ubuntu server. The task focused on applying the principle of defense in depth by configuring a host-based firewall (UFW) to block malicious traffic while allowing only legitimate connections. This exercise demonstrated how quickly an unsecured server can be compromised and why continuous monitoring and proactive security are essential.

## Objectives
- Understand the concept of the Attack Surface and the Principle of Least Privilege (PoLP).
- Perform a basic security audit of active network ports on a Linux server.
- Configure the Uncomplicated Firewall (UFW) with a Default Deny policy.
- Implement granular port management to selectively allow SSH and HTTP traffic.
- Document firewall rules and security best practices.
- Continue expanding my professional GitHub Cloud Computing Portfolio.

## Commands Executed
### Allow SSH
```bash
sudo ufw allow ssh
```
### Set Default Deny Policy
```bash
sudo ufw default deny incoming
sudo ufw default allow outgoing
```
### Allow Port 8080 (Web Application)
```bash
sudo ufw allow 8080/tcp
```
### Activate the Firewall
```bash
sudo ufw enable
```
### Check Firewall Status
```bash
sudo ufw status verbose
sudo ufw status numbered
```

## Skills Learned
- Practical application of host-based firewall security.
- Importance of minimizing the attack surface by managing open ports.
- How Default Deny policies enforce strict security baselines.
- Documentation of technical processes in Markdown for professional portfolios.
- Strengthened awareness of real-world risks when servers are left unsecured.
