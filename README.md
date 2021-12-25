<p align="center">
  <a title="Google CLoud" href="https://console.cloud.google.com" target="_blank">
    <img src="https://logosmarcas.net/wp-content/uploads/2021/03/Google-Cloud-Logo.png" width="400" alt="Google Cloud"/>
  </a>
</p>

## Language 🌐

* <img src="https://f.carlosdorelli.com.br/img/flags/usa.png" alt="USA Flag" width="25" height="15"> English (current)
* <img src="https://f.carlosdorelli.com.br/img/flags/br.png" alt="Brazil Flag" width="25" height="15"> [Português Brasileiro](/README.PT-BR.md) 

## GCloud SSH Login ☁

A list of necessary commands to allow root SSH login in your GCloud Plataform VM.

## How to use it 🤔
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

## Watch it 🎥
https://youtu.be/dVslkCrMr0Y

## Contributing 😉
If you find any error please tell me on my Discord (**Carlos Dorelli#9932**) that I will fix it.
