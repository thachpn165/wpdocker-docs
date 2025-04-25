# wpdocker backup website

Backup website source + DB

## Usage

```bash
wpdocker backup website DOMAIN STORAGE [RCLONE_STORAGE]
```

## Arguments

#### *DOMAIN*

Domain to be backed up

| Attributes      | &nbsp;
|-----------------|-------------
| Required:       | ✓ Yes

#### *STORAGE*

The storage type that will store the backup (e.g. local, rclone)

| Attributes      | &nbsp;
|-----------------|-------------
| Required:       | ✓ Yes

#### *RCLONE_STORAGE*

The storage name rclone will store this backup data, only declare if STORAGE=rclone is declared


