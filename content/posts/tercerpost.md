+++
title = 'INSTALACIÓN MONGODB EN DEBIAN 13'
date = 2025-10-02T12:19:51+02:00
draft = false
+++	

## 1. Actualizamos repositorios y hacemos las actualizaciones de los programas necesarios: 
  
- `sudo apt update`  
- `sudo apt upgrade`  


## 2. Instalamos dependencias necesarias

`sudo apt install -y gnupg curl wget software-properties-common apt-transport-https ca-certificates`

## 3. Añadimos el certificado de Mongo:

`curl -fsSL https://www.mongodb.org/static/pgp/server-7.0.asc | sudo gpg -o /usr/share/keyrings/mongodb-server-7.0.gpg --dearmor`

## 4. Ejecutamos el comando que instala el paquete que necesitamos:  

- `sudo apt install mongodb-org`  
  
- `sudo systemctl status `  

Debemos ver algo como *"active"* y eso significará que está correcto y funcionando.  

#### Si no está activo lo iniciamos:  
  
`sudo systemctl start mongod`
`sudo systemctl enable mongod`
  
## 5. Para acceder:
  
`mongosh`  

![Mongo](/images/mongo.png)  

[Acceso a página oficial](https://www.mongodb.com/)
