# chirpd

## Set up instructions (as root):

### Create a chirp user
```
# adduser chirp -c "Chirp user" -d /var/spool/chirp -s /sbin/nologin
```

### Copy etc to the system
```
cp -r etc/* /etc
```

### Start the daemon
```
service start chirpd
```
