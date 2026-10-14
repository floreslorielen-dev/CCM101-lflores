# Backup Script Guide

## Full Script Code
```bash
#!/bin/bash
# Automated Backup Script for CloudNova Technologies

SOURCE_DIR="app-data"
BACKUP_DIR="backups"
TIMESTAMP=$(date +"%Y%m%d_%H%M%S")

echo "Initiating automated backup..."
mkdir -p $BACKUP_DIR
tar -czf $BACKUP_DIR/backup_$TIMESTAMP.tar.gz $SOURCE_DIR
echo "Backup completed successfully at $TIMESTAMP!"
```
- The command ```chmod +x backup.sh``` changed the file permissions to make the script executable.
Without this, Linux treats the file as plain text and prevents it from running as a program.

## Cron Expression
```0 2 * * * /root/backup.sh```
This cron job runs the `backup.sh` script automatically every night at **2:00 AM**.  
Here’s the breakdown of each field:

- **0** → Minute (run at the 0th minute)  
- **2** → Hour (run at 2 AM)  
- **\*** → Day of Month (every day)  
- **\*** → Month (every month)  
- **\*** → Day of Week (every day of the week)
