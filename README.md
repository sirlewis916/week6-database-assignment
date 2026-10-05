# PostgreSQL Backup, Recovery and Streaming Replication

## Project
Bootcamp database backup and recovery for PLP Academy.

## Environment
- Windows
- PostgreSQL 18
- Database: `bootcamp`
- Table: `students`
- Verified data: 1 row: `1 | Alice | Beginner`

## Step 1: Take and Verify a Logical Backup
Backup created with:
```bash
pg_dump -Fc -f /backups/bootcamp.dump bootcamp
pg_restore --list /backups/bootcamp.dump | head
