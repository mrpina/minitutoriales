# Package.json





> Usaremos `npm init` para poder iniciar el creador de fichero package.json 

> Para instalar todas las dependencias que hay dentro del paquete usaremos `npm install` y por defecto buscara las dependencias en el archivo.





### Instalar las dependencias

- Automática 

Usando el siguiente comando se instalara el paquete y se añadirá en el package.json

```bash
npm install express --save 
```



- Manual

Para poder instalar las dependencias tendremos que añadir lo siguiente y a indicarle que paquetes queremos usar.

```json
{
  "name": "locator",
  "version": "1.0.0",
  "description": "Finds the country of origin of the incoming request",
  "main": "index.js",
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1"
  },
  "keywords": [
    "ip",
    "geo",
    "country"
  ],
  "author": "Sammy sammy@your_domain (https://your_domain)",
  "license": "ISC",
  "dependencies": {
    "axios": "^0.19.0"
  },

    //Aqui se ponen las dependencias que se quieresn añadir 
  "devDependencies": {
    "eslint": "^6.0.0",
    "express": "^4.17.1"
  }
}
```

