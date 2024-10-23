# Hostsblock

Hostsblock es una herramienta útil en sistemas Linux para bloquear publicidad, rastreadores, malware y otros sitios no deseados a nivel del archivo hosts del sistema. Funciona descargando y combinando listas de bloqueo de varias fuentes y agregando esas entradas al archivo /etc/hosts, redirigiendo las solicitudes de esos dominios a 127.0.0.1 o 0.0.0.0, lo que hace que no se puedan resolver y así se bloqueen.

## Instalación

Clonamos el repositorio Hostsblock:

```
git clone https://github.com/gaenserich/hostsblock.git
cd hostsblock
```

Una vez descagado, debemos mover los archivos a sus directorios correspondientes:

```
sudo cp hostsblock /usr/local/bin/
sudo cp hostsblock.conf /etc/
sudo cp hostsblock.sh /etc/
```

Abrimos el archivo de configuración:

```
sudo nano /etc/hostsblock.conf
```
Aquí podrás ajustar parámetros como las fuentes de listas de bloqueo que desea utilizar (por ejemplo, listas de Adblock, MalwareDomainList, etc.) y definir la frecuencia con la que Hostsblock debería actualizarse.

