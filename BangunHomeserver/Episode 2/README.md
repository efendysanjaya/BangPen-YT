## Cek status Port 53(DNS):

```
lsof -i :53
```
```
netstat -tulpn | grep ":53 "
```

## Disable and stop the systemd-resolved service:

```
sudo systemctl disable systemd-resolved.service
sudo systemctl stop systemd-resolved.service
```
