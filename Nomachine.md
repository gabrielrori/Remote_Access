

# Nomachine
Guía basada en:

https://kifarunix.com/install-nomachine-on-rocky-linux-8/
https://techviewleo.com/install-nomachine-rdp-on-rocky-almalinux/
https://www.howtoforge.com/install-and-use-nomachine-on-centos-8/

--------------------------------------------------------------------------------------
## Instalación
Descargar con wget:
```sh
wget https://download.nomachine.com/download/7.7/Linux/nomachine_7.7.4_1_x86_64.rpm
```
Instalar con dnf
```sh
sudo dnf install ./nomachine_7.7.4_1_x86_64.rpm
```
Si se tiene internet, basta con una línea:
```sh
sudo dnf install https://download.nomachine.com/download/7.7/Linux/nomachine_7.7.4_1_x86_64.rpm
```

## Uso

1. Iniciar el servidor en la aplicación.
2. En security, desmarcar: require permission to let remote users connect.
3. En el cliente, acceder a la dirección del servidor.

--------------------------------------------------------------------------------------
