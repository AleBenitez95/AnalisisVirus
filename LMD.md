# LMD
Linux Malware Detect (LMD), también conocido como Maldet, es una herramienta de detección de malware diseñada específicamente para sistemas Linux. Está optimizada para detectar amenazas comunes en entornos de alojamiento compartido y servidores web. Maldet utiliza firmas de amenazas conocidas, junto con la capacidad de identificar patrones anómalos en archivos y procesos, lo que lo convierte en una solución popular entre administradores de servidores Linux.

## Instalación

Descargamos e instalamos LMD:

```
wget http://www.rfxn.com/downloads/maldetect-current.tar.gz
tar -xzf maldetect-current.tar.gz
cd maldetect-*
sudo ./install.sh
```

Actualizamos las firmas de malware:

```
sudo maldet --update
```

Ejecutamos el script en el directorio que deseamos escanear:

```
sudo maldet --scan-all /ruta/del/directorio
```

Y por último para ver los resultados del escaneo escribimos:

```
sudo maldet --report ID_DEL_REPORTE
```
