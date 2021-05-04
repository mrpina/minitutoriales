# Script Bash



Que no nos salga la terminal 

```powershell
@echo off
```







Saltarnos las líneas que ejecutar "con espacio"

````powershell
REM 
````



### Variables 

```` bash
Para declarar 
set

Para introducr por teclado 
set /p 

Para operar 
set /a 
````



### If

```powershell
if "valor" "operador" "valor" "resultado"
if %ERRORLEVEL% == 0 ECHO realizado correctamente
```



### operadores 

```bash
set /a res=%var1%+%var2%
```





### Comentarios



En bloques 

```bash
goto :start

:start
```

En linea 

````bash
REM Comentario 
````