# Git



> Descargar los cambios del repositorio `git pull`
>
> Descartar los cambios de un fichero `git reset --hard` 
>
> Seleccionar la rama `git checkout "rama" `
>
> Mostrar el estado de los ficheros y archivos `git status`



### Proceso para subir archivos a git 

*Para hacerlo por primera vez hay que ir mas abajo*


> 1. Añadir archivos modificados `git add "ficheros"`
>
> 2. Añadir un titulo a los cambios `git commit -m "mensaje"`
>
> 3. Subir todos los cambios `git push -u origin "rama"`





### Preparar entorno de trabajo y subir a git por primera vez

1. Usaremos `clone` para copiar el repositorio que queremos usara para trabajar.

```bash
git clone "link del repositorio 'https://...' "
```



2. Usaremos `init` para indicarle que estamos en un repositorio de git

```bash
git init
```



3. Usaremos `checkout` para seleccionar la rama a la que queremos subir los archivos 

```bash
git checkout 'rama'
```



4. Realizaremos un `add`  para seleccionar los ficheros que queremos para que se añadan al repositorio

   *Podemos usar punto "." para seleccionar todos los archivos que se ha modificado*

```bash
git add "ficheros"
```



5. Usaremos `commit` para indicar los cambios que hemos hechos en archivos y directorios

```bash
git commit -m "mensaje"
```



6. Usaremos `remote` para conectarnos al repositorio 

```bash
git remote add origin 'repositorio'
```



7. Usaremos `push` para subir todos los cambios

```bash
git push -u origin 'rama'
```





#### Comprobar estados de los archivos

- `git status`



#### Creamos rama 

- `git branch`



#### Borrar una rama 

```bash
// delete branch local
git branch -d localBranchName

// delete branch remoto
git push origin --delete remoteBranchName
```

#### Borrar archivos 

Se borra el archivo o la carpeta se usa `git add `, luego `git commit` y al final `git push`









