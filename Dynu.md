

# Dynu

Instalar el servidor OpenSSH: 
```sh
yum install openssh
```
Checkear el status del servicio SSH: 
```sh
systemctl status sshd
```
Inicializar SSH:
```sh
systemctl start sshd
```
Editar el archivo de configuración de SSH: 
```sh
sudo vi /etc/ssh/sshd_config
```
Reinicializar SSH:
```sh
systemctl restart sshd.service
```
Ingresar a la interfaz del router (generalmente http://192.168.1.1 o http://192.168.0.1) e ir a la sección de 'Port Forwarding'. Agregar una regla  para el puerto TCP 22 para ser enviado a la dirección IP interna de la computadora linux.

Obtener la dirección de IP interna
```sh
ifconfig -i. 
```

Crear un puesto DNS dinámico en un propio dominio registrándose en "Dynu Dynamic DNS Service" 
Instalar el paquete de Dynu

```sh
rpm -ivh https://www.dynu.com/support/downloadfile/30 
```
Ingresar al dominio creado desde un cliente SSH para tener acceso remoto a la computadora.
