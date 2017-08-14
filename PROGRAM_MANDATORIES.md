# Program mandatories

## Program structure

1. The program must have a function to trigger the credentials information. This action may be called more than once, the **asking_credentials** function.
1. The program must have the **do_everything** function, triggerend when everything is checked and the variables are provided. May be the backup function itself.
1. The backuped file must be in the following format: $project_name.$time.
1. The backuped file will be a tar.gz.

## Functions

### asking_credentials

A function to ask the credentials.

### do_everything_function



## Variables names

### project_name

The poject name. Will identify the backup file.

### time

The expression to individualizes the backup by time. Will be in the following format:

```plain
<YEAR><MONTH><DAY>.<HOUR>h<MINUTE>m<SECOND>s
```

### backup_place

The current machine address to puth the backup.

### user_name

The ssh user name.

### user_password

The ssh user password.

### server_path

The ssh server path to files.

