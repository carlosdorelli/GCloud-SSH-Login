![Google Cloud SSH Login](https://i.imgur.com/SqHsYll.png)

Some commands to allow root SSH login in your GCloud Plataform VM.

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




3. Define a password to the user root using "passwd root"
4. Now its time to permit into the machine the login using root user, type "nano /etc/ssh/sshd_config"
5. Now that we are on sshd_config, lets permit the RootLogin and the PasswordAutentication. Go to "#ListenAddress ::" and add below "PermitRootLogin yes" then jump another line and add "PasswordAuthentication yes"
6. Now lets save and close the file - do Control X + Y + Enter
7. So then we restart the sshd service and it's done - "service sshd restart"
```

  
## Thanks 😉
If you find any error please tell me on my Discord (**Carlos Dorelli#8440**) that I will fix it.
