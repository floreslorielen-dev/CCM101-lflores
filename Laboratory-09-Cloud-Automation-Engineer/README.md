# Laboratory 09 – Cloud Automation Engineer

## Mission Overview
This mission focused on eliminating human error in cloud operations by automating the backup process.  
Using Bash scripting and Linux cron scheduling, I created a solution that automatically compresses and backs up application data every night at 2:00 AM.  
The activity emphasized the principle: *“If you have to do a task more than twice in the cloud, you should automate it.”*

## Objectives
- Understand Bash shell script syntax, variables, and basic commands.  
- Write and save executable scripts using the nano editor.  
- Modify Linux file permissions with `chmod`.  
- Schedule automated tasks using cron.  
- Document automation code and cron job configurations in Markdown.  
- Finalize the GitHub Cloud Computing Portfolio with automation capabilities.

## Commands Executed
```bash
# Create dummy data
mkdir app-data
echo "This is critical client data." > app-data/data.txt

# Write and edit script
nano backup.sh

# Make script executable
chmod +x backup.sh

# Run script
./backup.sh

# Verify backup
ls -l backups/

# Schedule cron job
env EDITOR=nano crontab -e
crontab -l
```
## Skills Learned
- Bash scripting fundamentals (variables, commands, shebang).
- Linux file permissions and execution rights.
- Cron job scheduling for automated tasks.
- Markdown documentation for technical processes.
- GitHub portfolio organization and version control.
