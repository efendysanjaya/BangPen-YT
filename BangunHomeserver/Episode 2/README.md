## YouTube Video

YouTube Link: [Episode 2](https://youtu.be/oksJH4e2IJA)

## Cek status Port 53(DNS):
```
sudo netstat -tulpn | grep ":53 "
```

## Disable and stop the systemd-resolved service:
```
sudo systemctl disable systemd-resolved.service
sudo systemctl stop systemd-resolved.service
```
