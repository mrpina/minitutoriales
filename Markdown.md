# Markdown

En este documento introduciremos las sintaxis mas importantes de markdown

## Títulos y encabezados   

Los títulos y los encabezados funcionan de la misma manera. Dependiendo del numero de `#` que pongas el tamaño del encabezado y la importancia del titulo cambiara.

# Titulo y encabezado  1

- `# Titulo y encabezado 1`

## Titulo y encabezado 2

- `## Titulo y encabezado 2`

### Titulo y encabezado 3

- `### Titulo y encabezado 3`

#### Titulo y encabezado 4

- `#### Titulo y encabezado 4`

###### Titulo y encabezado 5

- `###### Índice 5`

---

# Listas 

Aquí tenemos todos los ejemplos de listas que se pueden hacer.

- Lista 1
+ Lista 2

* Lista 3 

1. Lista 4

```markdown
- Lista 1
+ Lista 2
* Lista 3
1. Lista 4
```



## Sublistas

- Lista 1
  - Sublista 1

+ Lista 2
  + Sublista 2

* Lista 3 
  * Sublista 3

1. Lista 4
   1. Sublista 4

```markdown
- Lista 1
  - Sublista 1

+ Lista 2
  + Sublista 2

* Lista 3 
  * Sublista 3

1. Lista 4
  1. Sublista 4
```

## Lista de tareas 

- [x] Tarea 1
- [ ] Tarea 2
- [x] Tarea 3



```markdown
- [x] Tarea 1
- [ ] Tarea 2
- [x] Tarea 3
```

---

## Añadir código

Para poder añadir código tenemos que usar ` ` `

- `Esto es código ` 

Al añadir bloques de código nos da la opción de elegir el lenguaje y si nuestro interprete de markdown en compatible le añadirá los colores al código

Tenemos 2 maneras de hacerlo 

- Con los acentos cerrados

```markdown
​``` "Lenguaje"
	
	"Codigo"

​``` 
```

  

- Con las virgulillas ~

```t
~~~ "Lenguaje" 
	
	"Codigo"

~~~
```

   

---

## Atributos al texto 

#### Simples 

- **Negrita** 
  - `**Negrita** `
- __Negrita__
  - `__Negrita__`
- *Cursiva*
  - `*Cursiva*`
- _Cursiva_
  -	`_Cursiva_`
- ~~Tachado~~
  - `~~Tachado~~`

### Combinados 

- ***Cursiva negrita***
  
  - `***Cursiva negrita***`
- ___Cursiva negrita___
  
  - `___Cursiva negrita___`
  
  

---

## Tabla 


|      | a    | b    | c    | d    |
| ---- | ---- | ---- | ---- | ---- |
| 1    |      |      |      |      |
| 2    |      |      |      |      |
| 3    |      |      |      |      |



```markdown
|      | a    | b    | c    | d    |
| ---- | ---- | ---- | ---- | ---- |
| 1    |      |      |      |      |
| 2    |      |      |      |      |
| 3    |      |      |      |      |
```

---

## Link

- [Link abreviado](https://www.google.es)
  - `[Link abreviado](https://www.google.es)`
- <http://www.google.es>
  - `<http://www.google.es>`

---

## Imagenes 

![Palamera](palmera.jpg)

---
## Extras 

- Para poner la barra solo tenemos que escribir `---`

  ---
