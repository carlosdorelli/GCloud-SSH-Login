# GCloud
Step 1: Login SSH and Su Root 
sudo su root

Step 2: Change password Root
passwd root

Step 3: Config SSHD allow Root login
nano /etc/ssh/sshd_config

PermitRootLogin yes

PasswordAuthentication yes

service sshd restart
