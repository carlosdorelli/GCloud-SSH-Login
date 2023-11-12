![Google Cloud SSH Login](https://i.imgur.com/SqHsYll.png)

Some commands to allow root SSH login in your GCloud Plataform VM. It's recommended to use SSH Keys but if you need log into root not by SSH keys follow the steps below. Join my Discord Server to more repositories [Dorelli's Server](https://discord.gg/jXhRKPxAuM).

## Commands

Access your SSH terminal via GCloud Plataform

Type
```
su root
```
and you will get into root user.

Now we gonna define a password to root typing
```
passwd root
```

Allowing SSH External login
```
nano /etc/ssh/sshd_config
```

Go to "#ListenAddress ::" and add below
```
PermitRootLogin yes
PasswordAuthentication yes
```
Save and exit

Restart the SSHD service
```
service sshd restart
```
It's done.

## Contribute
Para qualquer alteração abra uma discussão.
