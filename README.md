# RsyncBackups
Script collection used to automate Rsync backups to a local fileserver

- "battcheck" is called by a cron job to initiate the process. Checks the battery level and runs the script if OK.
- "battcheck-low" is run if the battery level is too low to Rsync. If the laptop is still not plugged in before then, the whole process ends.
- "rsync-backup" is run when the battery level is above 20%. This will use Rsync via SSH to a server with Key Auth
- "battcheck-ok" is run when the Rsync finishes successfully
