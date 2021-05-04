# Programar en bash 

---

> Datos básicos
>
> Para que se ejecute tiene que estar entre 2 paréntesis `(())`
>
> Para terminar la ejecución del script que lo añadiremos dependiendo de lo que tenemos planeado que pasara si sale de una manera o otra
>
> + `exit 1`
>   + Salida con éxito
> + `exit 2`
>   + Salida con errores 
> + `exit 3`
>   + Uso indebido 

---

## Variables, operaciones aritméticas y operaciones lógicas 

> Para ver las variables locales `env` o `printenv` para usarla `$variable`



> Para declarar variables globales 

```bash
myvar='dato'
echo $myvar
```



> Para poder declarar y eliminar variables persistentes

```bash
# Declarar
export my_var='datos'
#Eliminar
unset myvar
```



> Para almacenar comandos en una variable `mydir=$(pwd)`

> Para realizar operaciones aritméticas
>
> ```bash
> #Operaciones en variables y que se calcule
> suma=$((1+1))
> 
> suma=1+1
> resta=1-1
> multi=1*1
> div=1/1
> 
> #Resto de la división
> rest=1%1
> ```



> Operaciones aritmeticologicas
>
> ```bash
> -lt = Menor
> -le = Menor o igual
> -eq = Igual
> -ge = Mayor o igual
> -gt = Mayor
> -ne = Distinto 
> 
> <  = Menor
> <= = Menor o igual
> == = Igual
> >= = Mayor o igual
> >  = Mayor
> !  = Distinto
> 
> || = o una o la otra 
> && = esto y esto 
> ```



> Operadores incrementales
>
> ```bash
> #Cada vez que se ejecuta se añadira y borrara 1 respectivamente a la variable
> i=$((i+1))
> i=$((i-1))
> 
> #Es la manera abrevidad de hacer un incremental de +1 o -1
> #Incrementa el primer valor 
> ++i
> #incrementa el ultimo valor 
> i++
> 
> #Decrementa el primer valor 
> --i
> #Decrementa el ultimo valor 
> i--
> ```
>
> 

---

## Array, diccionarios

> Las array tienen como primer valor el 0 
>
> La variable para una array se indica con paréntesis `array_var=()`
>
> + Se pueden hacer secuencias sin aplicar los caracteres 1 a 1 `array_var=( {1..20} {a..z} {20..1})`
>
> Para poder añadir o remplazar la información de una tenemos que indicarlo de esta forma `array_var[0]="Array1"`
>
> Para poder ver la informacion de  la array usaremos:
>
> + Para poder ver un valor `echo ${array_var[0]}` 
> + Para ver todos los valores `echo ${array_var[*]}`
> + Para ver valores en secuencia `echo ${array_var[0..9]}`

---

## Bucles While y for 

> #### Datos
>
> _Todos los datos que le entran al for usa el valor que tiene o los numera y esta numeración es el numero de iteraciones que realiza el bucle_
>
> _Todos los bucles se pueden realizar de forma inversa pero en vez de sumar a la variable se tiene que restar_
>
> _Para finalizar los bucles usaremos `break` y para continuarlos `continue` que se salta la iteración_



> Bucle while
>
> Usaremos el `do` para ejecutar los bules y `done` para terminarlo
>
> ```bash
> #Variable donde se guarda la información del ciclo del bucle 
> i=0
> 
> #Compara si la variable $i es menor que el valor 10 si lo es el bucle se repite 
> while [ $i -lt 10 ]
> do
>     echo 'Texto que se repite'
>     ((i++))
> done
> ```
>
> 



> Bucle while infinito
>
> ```bash
> 
> while : do
>     echo "Bucle infinito"
>     #sleep determina el tiempo que tardara en acabar el bucle 5 segundos en este caso
>     sleep 5
> done
> ```
>
> 



> Bucle for 
>
> 
>
> ```bash
> #Realizara el bucle hasta que la variable i llegue a 1000
> for i in {1..1000}
> do
>     echo "$i.Texto repetido"
> done
> ```
>
> 
>
> ```bash
> #Podemos realizar las operaciones de manera manual lo que nos permite personalizar el bucle 
> for ((i=1;i<=1000;i++))
> do
>     echo "$i.Texto repetido"
> done
> ```
>
> 
>
> Se puede realizar bucles con las salidas de los comandos 
>
> ```bash
> for i in $(ls)
> do
>     echo $i
> done
> ```
>
> 
>
> Ejemplo interesante 
>
> ```bash
> #Realiza el bucle y uestra las 3 palabras una detras de otras 
> for color in rojo amarillo verde
> do
>     echo "Este es el color $color"
> done
> ```

---

## Condicionales IF...Else y try catch

> Para comparar cadenas de caracteres tenemos que indicar la variable `$var = 'texto'` y la comparación con comillas  `if [ "$var" = "texto" ]`

---

## Funciones 









#### Añadir 

+ input de información

   



