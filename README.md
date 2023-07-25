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
