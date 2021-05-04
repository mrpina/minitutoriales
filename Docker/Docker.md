# Docker WSL

### Comandos básicos 

> Ver la versión `docker -version` 
>
> Ver todos los contenedores  `docker ps -a `
>
> Ejecutar comandos en un contenedor `docker exec -it "contenedor" "comandos"`

 

### Descargar una imagen 

- Usando un comando para descargar la imagen o a la hora de iniciar el contenedor también se descarga automáticamente.

> Para descargar una imagen `docker pull 'imagen'` 



### Creando contendor con comando 



> `docker run -it --rm dockerfile/ubuntu`

### Crear un contenedor 

- Para crear un contenedor usaremos [docker-compose](Docker_compose.md)





### Todos los contenedores

- Iniciar todos los contenedores 

  > `docker start $(docker ps -a -q)`

- Parar todos los contenedores 

> `docker stop $(docker ps -a -q)`  

- Borrar todos los contenedores 

> `docker rm $(docker ps -a -q)`  

- Borrar todas las imágenes 

> `docker rmi $(docker ps -a -q)`  

  
