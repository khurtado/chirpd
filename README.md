# chirpd

Set up instructions:

- Create a chirp user
adduser chirp -c "Chirp user" -d /var/spool/chirp -s /sbin/nologin

- Create /var/chirp/hadoop backend
mkdir -p /var/chirp
cd /var/chirp
cp -r /usr/lib/hadoop/ .
cp /usr/lib64/libhdfs* hadoop/lib/
