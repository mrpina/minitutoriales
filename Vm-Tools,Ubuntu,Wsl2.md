# Vm-Tools, Ubuntu & Wsl2



## Vm-Tools



#### Usando la iso de vmware-tools

> Copiamos el fichero y lo guardamos en el escritorio

`cp VMwareTools.x.x.x-xxxx.tar.gz ~/Escritorio`

> Para poder extraerlo usaremos el comando tar

`tar -xvf VMwareTools.x.x.x-xxxx.tar.gz`

> Entraremos en la carpeta que hemos extraído

`cd vmware-tools-distrib`

> Para instalarlo usaremos el archivo `sudo ./vmware-install.pl ` y lo ejecutaremos. 

#### Usando Open-tools

_Solo testeado en VmWare_

> Tendremos que descargarlo directamente desde apt y no requiere configuración 

`sudo apt install open-vm-tools-descktop`



## Ubuntu

> Cambiar el idioma del teclado 
>
> - `dpkg-reconfigure keyboard-configure`



## Wsl2

#### Ficheros

- passwd

#### Errores de compatibilidad

Los comandos de a continuación no funcionan

> + systemctl

#### Apagar

- Desde powershell ponemos 

> `wsl --shutdown`