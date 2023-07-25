# Xubuntu-22.04-Cheat-Sheet

## Autologin

```bash
sudo nano /etc/lightdm/lightdm.conf
```

```
[Seat*:]
autologin-guest=false
autologin-user=your-username-here
autologin-user-timeout=0
autologin-session=lightdm-autologin
```

## Wireguard

Install needed packages:

```bash
sudo apt update && sudo apt install wireguard openresolv
```

Paste in the the result of `pvpn get your-new-machine-name.your-vpn-domain` from the server here:

```bash
sudo vi /etc/wireguard/vpn0.conf
```

Auto start

```bash
sudo systemctl enable wg-quick@vpn0.service
```
