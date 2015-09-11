- Configuration file to set aws secrets, backup schedules etc.  Will use the standard AWS credential storage.  Will use the "http://169.254.169.254/latest/meta-data/instance-id" type URLs to fill in required fields.

- Setup cmdlet to check / configure IAM policy, scheduled task etc.

- Backup cmdlet to run sync.exe and create a snapshot of each volume (if required for that day - idempotent), tagged appropriately

- Purge cmdlet to delete unneeded snapshots

- Status cmdlet to show status of backup snapshots for all volumes

- Integrate volume expanding script?

- Think hard about monitoring system to make sure backups are running and up to date