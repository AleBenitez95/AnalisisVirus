# RootkitHunter

### Instalación

````
sudo apt-get install rkhunter
````
### Actualización

Actualización de base de datos de rkhunter

````
sudo rkhunter --update
````

### Comprobación

````
sudo rkhunter --check
````

![Warning](img/img2.png)

Toda la información se quedará guardada en /var/log/rkhunter.log

Para verlo solo tenemos que escribir:

````
sudo cat /var/log/rkhunter.log
````
Para verlo de manera interactiva con el terminal escribiremos:

````
sudo less /var/log/rkhunter.log
````






