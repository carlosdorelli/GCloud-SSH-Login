[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity)
![Maintainer](https://img.shields.io/badge/maintainer-carlosdorelli-blue)
[![Linux](https://svgshare.com/i/Zhy.svg)](https://svgshare.com/i/Zhy.svg)
[![GitLab last commit](https://badgen.net/gitlab/last-commit/NickBusey/HomelabOS/)](https://gitlab.com/NickBusey/HomelabOS/-/commits)
[![Discord](https://img.shields.io/discord/984111282556903544.svg?label=&logo=discord&logoColor=ffffff&color=7389D8&labelColor=6A7EC2)](https://discord.gg/Ew2MdZEMzz)

A list of necessary commands to allow root SSH login in your GCloud Plataform VM.

---

## Let's go 😎
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

---

## Fast Copy and Paste ⌨
```sh
sudo su root
passwd root
nano /etc/ssh/sshd_config
# Add these two lines below #ListenAddress ::
PermitRootLogin yes
PasswordAuthentication yes
service sshd restart
```

---
  
## Thanks 😉
If you find any error please tell me on my Discord (**Carlos Dorelli#8440**) that I will fix it.
