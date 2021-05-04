# Instalar Minecraft Server

### Instalar Java

Lo primero que tenemos que hacer es instalar openjdk

+ > `sudo apt install default-jdk`

  

_Si es un server con mods solo he podido hacerlo funcionar con openjdk-8_

+ > `sudo apt-get install openjdk-8-jdk`

Comprobar la versión de java 

+ > `java --version`



### Descargar el server
Descararemos el link del server con el comando `wget` 

+ > `wget` _Link del server_

_Link abajo para instalar wget, unzip_



### Ejecutar el server

Lo primero tenemos que crear un archivo con el nombre `start.sh` 

+ > Dentro introduciremos el siguiente comando dentro `java -Xmx4G -Xms1024M -jar "nombre del server".jar nogui`



Para ejecutar el server para poder ejecutar realizaremos

+ Permisos para la ejecución del script que hemos creado antes `./start.sh` tendremos que añadirle los permisos necesarios 

  

  + > `sudo chmod 777 ./start.sh`



---

### Extras 
> La ip de la maquina virtual en wsl2 es la "eth0"

> El puerto por defecto es 25565

> Para descomprimir un zip necesitaremos instalar `sudo apt install unzip` y para descomprimirlo usaremos  `unzip "archivo".zip`

> Instalar wget `sudo apt-get install wget`