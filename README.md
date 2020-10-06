# About it
>This is the command list necessary to permit root SSH Login in your Ubuntu server (any version) hosted in GCloud Plataform.

## How to use it
```sh
1. Access your SSH Terminal via GCloud Plataform
2. Type "sudo su root" that will log you into root
3. Define a password to the user root using "passwd root"
4. Now its time to permit into the machine the login using root user, type "nano /etc/ssh/sshd_config"
5. Now that we are on sshd_config, lets permit the RootLogin and the PasswordAutentication. Go to "#ListenAddress ::" and add below "PermitRootLogin yes" then jump another line and add "PasswordAuthentication yes"
6. Now lets save and close the file - do Control X + Y + Enter
7. So then we restart the sshd service and it's done - "service sshd restart"
```
Now it's just login into your Virtual Machine using the user root and the password you wrote in the third step.

## Get in contact
If you have any doubt just contact me by Discord "Eldremor#0001".
