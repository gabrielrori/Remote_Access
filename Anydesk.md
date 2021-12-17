

# Anydesk
Guía basada en:

https://techviewleo.com/install-anydesk-on-rocky-almalinux/
https://www.how2shout.com/linux/how-to-install-anydesk-on-rocky-linux-8/
https://www.linuxcompatible.org/story/how-to-install-anydesk-on-centos-8/
https://otodiginet.com/software/how-to-install-anydesk-on-centos-8/

--------------------------------------------------------------------------------------
## Instalación
Agregar el repositorio de Anydesk a linux con los siguientes comandos:
```sh
sudo tee /etc/yum.repos.d/anydesk.repo<<EOF
[anydesk]
name=AnyDesk CentOS - stable
baseurl=http://rpm.anydesk.com/centos/x86_64/
gpgcheck=1
repo_gpgcheck=1
gpgkey=https://keys.anydesk.com/repos/RPM-GPG-KEY
EOF
```
Se crea un archivo de repositorio en /etc/yum.repos.d/anydesk.repo:
```sh
cat /etc/yum.repos.d/anydesk.repo
```
Habilitar respositorio epel:
```sh
sudo yum -y install epel-release
```
Ahora que el repositorio se encuentra agregado, instalar:
```sh
sudo yum install anydesk
```
--------------------------------------------------------------------------------------
