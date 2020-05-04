## Database commands

```bash
# Capture and download
heroku pg:backups:capture
heroku pg:backups:download

# Restore
pg_restore --verbose --clean --no-acl --no-owner -h localhost -U [USER] -d diffengine [DUMP_FILE]

# Reset online
heroku pg:reset DATABASE --confirm [APP_NAME]
```