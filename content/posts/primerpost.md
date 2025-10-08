+++
title = 'INSTALACIÓN MARIADB EN DEBIAN 13'
date = 2025-10-02T12:19:51+02:00
draft = false
+++	

## 1. Actualizamos repositorios e instalamos actualizaciones.  
  
- Así actualizamos los repositorios: `sudo apt update`  
- De esta manera actualizamos lo que haya pendiente: `sudo apt upgrade`  
  
## 2 .Instalamos los paquetes necesarios:


`sudo apt install mariadb-server mariadb-client`  
  
## 3 .Confirmamos que está disponible para usar:
  
`sudo systemctl status mariadb`  
`sudo systemctl start mariadb`  
`sudo systemctl enable mariadb`  

## 4 .Si queremos configurar y entrar  
  
`sudo mysql_secure_installation`  
  
Y pulsamos *yes* a todo.   
  
Para acceder:   

`sudo mariadb -u usuario -p `  

![Mariadb](/images/mariadb.png)  
Para acceder a la página oficial: 

[Pagina oficial MariaDB](https://mariadb.org/) 
