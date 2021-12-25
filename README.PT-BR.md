<p align="center">
  <a title="Google CLoud" href="https://console.cloud.google.com" target="_blank">
    <img src="https://logosmarcas.net/wp-content/uploads/2021/03/Google-Cloud-Logo.png" width="400" alt="Google Cloud"/>
  </a>
</p>

## Língua 🌐

* <img src="https://f.carlosdorelli.com.br/img/flags/br.png" alt="Bandeira do Brasil" width="25" height="15"> Português Brasileiro (atual)
* <img src="https://f.carlosdorelli.com.br/img/flags/usa.png" alt="Bandeira dos Estados Unidos" width="25" height="15"> [English](/README.md) 


## GCloud SSH Login ☁

Uma lista de comandos necessários para permitir o login root via SSH na sua máquina da Google Cloud.

## Como usar? 🤔
```sh
1. Acesse o terminal SSH da sua máquina
2. Escreva "sudo su root" que vai te logar no usuário root
3. Defina uma senha para o usuário através do comando "passwd root"
4. Agora nós vamos permitir o login nas configurações da máquina com o comando "nano /etc/ssh/sshd_config"
5. Vá até "#ListenAddress ::" e na linha de baixo adicione "PermitRootLogin yes". Debaixo dessa nova linha, faça o mesmo para "PasswordAuthentication yes"
6. Agora é só salvar e fechar através de - Control X + Y + Enter
7. Agora é só reiniciar o serviço sshd e pronto - "service sshd restart"
```

Agora é só fazer login na sua Máquina Virtual usando o usuário root e a senha criada no terceiro passo.

## Copie e cole rápido ⌨
```sh
sudo su root
passwd root
nano /etc/ssh/sshd_config
# Adicione essas duas linhas embaixo de #ListenAddress ::
PermitRootLogin yes
PasswordAuthentication yes
service sshd restart
```

## Assista 🎥
https://youtu.be/dVslkCrMr0Y

## Contribua 😉
Se você encontrar algum erro é só me informar no Discord (Carlos Dorelli#9932) que eu arrumo.
