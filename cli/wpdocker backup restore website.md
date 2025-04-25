# wpdocker backup restore website

Restore website source + DB

## Usage

```bash
wpdocker backup restore website DOMAIN CODE_BACKUP_FILE DB_BACKUP_FILE
```

## Arguments

#### *DOMAIN*

The domain will perform full data recovery (including source code and database)

| Attributes      | &nbsp;
|-----------------|-------------
| Required:       | ✓ Yes

#### *CODE_BACKUP_FILE*

The path to the backup file for the site

| Attributes      | &nbsp;
|-----------------|-------------
| Required:       | ✓ Yes

#### *DB_BACKUP_FILE*

The path to the database backup file

| Attributes      | &nbsp;
|-----------------|-------------
| Required:       | ✓ Yes


