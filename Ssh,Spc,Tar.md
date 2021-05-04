# Ssh, Scp y Tar



### Conexión ssh 

Para poder conectarnos necesitaremos la ip y el usuario. _Si no lo queremos poner se  pondrá el usuario por defecto si solo hay 1_

`ssh usuario@ip`



### Descargar archivos y carpetas desde SCP

> Para descargar carpetas usaremos el mismo comando pero con `-r` delante de la conexión 

`scp usuario@ip_servidor:ruta_del_recurso ruta_destino`

### Subir archivo o carpeta desde SCP

`scp recurso usuario@ip_servidor:ruta_de_destino`



### Tar 

- Comprimir directorios 

`tar -zcvf "nombre del archivo comprimido" "nombre del directorio a comprimir"`



- Descomprimir directorios 

`tar -xvzf "archivo a descompriimir "`