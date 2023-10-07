# wireguard-setup
```bash
sudo apt install wireguard-tools resolvconf
```

copy the `conf` file to `/etc/wireguard/`

```bash
sudo su
cp Adi.conf /etc/wireguard/
```

wireguard up
```bash
sudo wg-quick up Adi
sudo wg-quick save Adi
```

for wireguard to be automatically up, everytime you turn on your system
```bash
sudo systemctl enable wg-quick@Adi
```
