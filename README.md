# About it
>This is only the commands to permit root SSH Login in your Ubuntu server (any version).

## The commands
```
sudo su root
passwd root
nano /etc/ssh/sshd_config
PermitRootLogin yes
PasswordAuthentication yes
service sshd restart
```
