+++
title = 'INSTALACIÓN POSTGRESQL EN DEBIAN 13'
date = 2025-10-02T12:19:51+02:00
draft = false
+++	

## 1. Actualizamos repositorios y hacemos las actualizaciones de los programas necesarios: 
  
- `sudo apt update`  
- `sudo apt upgrade`  

## 2. Ejecutamos el comando que instala el paquete que necesitamos:  

- `sudo apt install postgresql postgresql-contrib`  
  
- `sudo systemctl status postgresql`  

Debemos ver algo como *"active"* y eso significará que está correcto y funcionando.  

#### Si no está activo lo iniciamos:  
  
`sudo systemctl start postgresql`
`sudo systemctl enable postgresql`
  
## 3. Para acceder:
  
`sudo -iu postgres psql`  

![Postgresql](/images/postgresql.webp)  

[Acceso a página oficial](https://www.postgresql.org/)
