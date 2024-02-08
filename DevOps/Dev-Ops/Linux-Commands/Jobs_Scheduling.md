
### At Command
Linux **at command** is used to **schedule a task** to execute it once at a specified time, without editing a configuration file. It is an alternative to **the cron job scheduler.** It can be useful if we want to execute a process after some time, such as a shutdown system, taking backups, sending emails as reminders, and more.
Name of Service
**atd**
```bash
1. systemctl start atd  
2. systemctl enable atd
```

at (Time schedule)
atq: List of all jobs
atrm #: Remove the Job

