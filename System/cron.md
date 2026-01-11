# Cron

### Cron is a time based job scheduler.
### It runs in background and executes tasks at specified time.

## Use
- Automating backups, log rotation monitoring
- Running scripts for testing or deployment 
- Cleaning temporary files, updating packages

### Cron jobs are defined in a crontab file uing syntax

```bash
* * * * * command
```
- Each * reprents:
- Minute(0-59) | Hour(0-23) | Day of month(1-31) |Month(1-12) | Day of Week(0-6,sunday=0)
- Example
```bash
0 2 * * * /usr/bin/backup.sh  # Runs backup at every day at 2:00 AM
```

### Restricting Cron Access
### Unrestricted cron acess can cause security risks.

- List users allowd access /etc/cron.allow

- List users denied access /etc/cron.deny

- Monitor cron logs (/var/log/cron) to detect unysyal activity.

### Practice
```bash
crontab -l  # Check if cron is installed

crontab -e  # Opens an editor, here you will add your schedule jobs 

```
### My First cron job
```bash
* * * * * echo "Hello Cron $(date)" >> /home/ravigoyal/cron_test.log
```
```bash
0  Minute  -> Runs 0 minute of the hour 
*  Hour    -> Every hour 
*  Day of the month -> Every day 
*  Month   -> Every month 
*  Day of the week -> Every day of the week
```
```bash
 0 * * * * notify-send "Take a Break" # Cron will run at the start of every hour

```
```bash
0 0 * * 0 rm ~/Downloads/temp/* # Clean temporary Files 
```

