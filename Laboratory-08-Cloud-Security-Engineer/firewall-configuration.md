# Firewall Configuration – Laboratory 08

## Commands Used to Secure the Server

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
