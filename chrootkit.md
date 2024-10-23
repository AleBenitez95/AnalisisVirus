# chrootkit

chkrootkit es una herramienta de seguridad para sistemas Linux que se utiliza para buscar la presencia de rootkits en el sistema. Un rootkit es un conjunto de herramientas utilizadas por un atacante para obtener acceso no autorizado a un sistema informático, y puede ser difícil de detectar y eliminar. chkrootkit puede ayudarte a identificar la presencia de estos rootkits, así como otros tipos de malware.

## Instalación

```
sudo apt update
sudo apt install chkrootkit
```

Ejecutamos chrootkit como root:

```
sudo chkrootkit
```
```
Checking 'apm'...                 Not infected
Checking 'basename'...            Not infected
Checking 'chfn'...                Not infected
Checking 'chsh'...                Not infected
Checking 'cron'...                Not infected
Checking 'du'...                  Not infected
Checking 'ifconfig'...            Not infected
Checking 'inetd'...               Not infected
Checking 'init'...                Not infected
Checking 'lkm'...                 Not infected
Checking 'login'...               Not infected
Checking 'ls'...                  Not infected
Checking 'mknod'...               Not infected
Checking 'mount'...               Not infected
Checking 'netstat'...             Not infected
Checking 'rarp'...                Not infected
Checking 'rlogin'...              Not infected
Checking 'syslogd'...             Not infected
```
**INFECTED:** Indica que se ha encontrado un posible rootkit.

**Not infected:** Indica que no se ha encontrado nada sospechoso.


