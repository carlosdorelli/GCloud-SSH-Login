# GCloud
sudo su root

passwd root

nano /etc/ssh/sshd_config

PermitRootLogin yes

PasswordAuthentication yes

service sshd restart
