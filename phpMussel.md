# phpMussel
phpMussel es un script PHP diseñado para detectar troyanos, virus, malware y otras amenazas dentro de los archivos cargados en su sistema donde quiera que se encuentre el script. 

## Instalación
Descargamos el respositorio 
```
wget https://github.com/phpMussel/phpMussel/archive/refs/heads/master.zip
```
Descomprimimos el archivo comprimido y entramos en el directorio
```
unzip master.zip
cd phpMussel-master
```
Y copiamos el script a donde se encuentra el proyecto web

```
cp -r phpMussel /var/www/html/
```
Y por último lo integramos:

```
<?php
require_once '/ruta/a/phpMussel/loader.php'; // Incluye phpMussel.

$phpMussel = new phpMussel(); // Instancia phpMussel.

// Ruta del archivo que se va a cargar.
$filePath = '/ruta/al/archivo/subido';

// Ejecuta el escaneo.
$phpMussel->Scan($filePath);

// Si detecta alguna amenaza.
if ($phpMussel->ThreatFound) {
    echo 'Archivo malicioso detectado y bloqueado.';
} else {
    echo 'Archivo seguro.';
}
?>
```
