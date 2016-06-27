# chirpd

## Set up instructions (as root):

### Create a chirp user
```
# adduser chirp -c "Chirp user" -d /var/spool/chirp -s /sbin/nologin
```

### Add chirp certificates
# mkdir /etc/grid-security/chirp
# cp /etc/grid-security/hostcert.pem /etc/grid-security/hostkey.pem /etc/grid-security/chirp
# chown -R chirp:chirp /etc/grid-security/chirp

### Copy etc to the system
```
cp -r etc/* /etc
```

### Start the daemon
```
service start chirpd
```
