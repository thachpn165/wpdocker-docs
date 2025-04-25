# wpdocker backup cleanup

clean up backups older than x days

## Usage

```bash
wpdocker backup cleanup DOMAIN MAX_AGE_DAYS
```

## Arguments

#### *DOMAIN*

Domain needs to clean up its backup

| Attributes      | &nbsp;
|-----------------|-------------
| Required:       | ✓ Yes

#### *MAX_AGE_DAYS*

Maximum number of days old of backup files allowed to be retained (e.g. 7 will delete files older than 7 days)

| Attributes      | &nbsp;
|-----------------|-------------
| Required:       | ✓ Yes


