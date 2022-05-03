

# :book:  Tercer clase : 26 abril - GIT

---

## :star: Los 3 estados de GIT

Recordatorio de la clase anterior

Vimos los comandos:

```
•Git Status
•Git Add
•Git Commit
•Git Log
```

---

## :star: Modificaciones de Carpetas

#### ¿Qué pasa cuando modificamos algún archivo que ya habíamos commiteado?

- Si en nuestra área de trabajo hemos agregado algún archivo nuevo, al ejecutar **git status** ya estando dentro de nuestra carpeta Git, nos aparecerán en **rojo** esa modificaciones.

- Con **git status** comprobamos el estado de nuestra carpeta Git

- Una vez que nos aparecen las modificaciones ya podemos agregarlas a nuestra área de trabajo
con **git sdd .** para mover **todos** los archivos o sino con  **git add «nombre del archivo»** para pasar sólo por nombre.

- Los archivos ya están listos para ser commiteados.

- **git commit – m «para escribir mensajes cortos»**. 

- **git commit**  nos abre el editor que por defecto tenga su máquina, para escribir mensajes un poco más extenso.

Al finalizar:
```
Ctrl. + S( guardamos mensaje de texto ) 
Ctrl. + X(salimos del editor)
```

Otra opción es tecleamos Esc. y al final del editor nos aparecen : tecleamos wq!( nos guarda nuestro texto y salimos del editor Vim)

### ¿Cómo diferenciamos un archivo de una carpeta en la terminal de Git Bash?

```
  / nombre archivo
../indica que hay dos carpetas o una carpeta superior
```



### :star: ¿Cómo guardar modificaciones en un Archivo?

- Para guardar las modificaciones que hemos hecho en algún archivo.

- Con:  **git commit –am  «agregué una línea a mi repositorio»**

- No me permite realizar commitear modificaciones en un mismo archivo.
                                                                                               ---
   
En la capeta tecnicatura Git realizar:

•Añadir desde cualquier editor de texto un archivo Readme.txt

•Visual Estudio Code

•Sublime Tex

•Block de notas

Creamos una subcarpeta Readme en al carpeta Tecnicatura Git, desde la terminal Git bash

Modificamos nuestro archivo agregando una línea de texto.

### Desde el editor de texto Vim:

-en la primer línea, escribimos nuestro comentario para el commit

-luego guardamos con Control S 

-salimos del editor con Control X

Creamos nuestra modificación en el repositorio

El último commit siempre aparece el principio y el primer commit al final, vemos la línea de commit con git log y luego salimos con q

**Ojo! cuando usamos el comando Git add .**


Git add . Agrega los archivos o modificaciones sólo  en la carpeta o subcarpeta  donde estamos ubicados.

Por ej: Si estamos ubicados en una subcarpeta y tecleamos Git add . No nos  agregara los archivos de otra subcarpeta donde no  estemos ubicados.

Con ```git commit -m « escribimos comentario para el commit» ``` luego nos aparece el commit, con la descripción de lo que hemos modificado.

Con ```git log```  vemos la línea de commit que se va formando, para salir tecleamos la letra  q

Cuando tenemos archivos modificados se puede utilizar el siguiente comando:

```git commit –am «escribimos el comentario de nuestro commit»```

No se puede utilizar con archivos nuevos.

Sólo con archivos modificados


---

### :star: Comando Git Checkout:


•El comando  ```git checkout``` me permite borrar archivos modificados.

•No me permite eliminar archivos nuevos.

•```git checkout <nombre del archivo>```

•```git checkout –f <mensaje>``` nos va a permitir borrar todos los últimos cambios realizados

---

### :star: Git RESTORE

``` git restore  --stage <nombre del archivo>```.

•Vuelve el archivo al área de trabajo y poder modificarlos

---

### :star: Comando  Git Diff

- Me permite saber qué agregué en el espacios de preparación.

- Nos muestra las modificaciones que hicimos en el archivo de nuestro repositorio.

- Este comando nos permite saber que tipo de modificaciones hicimos.

---

### :star: Git Diff --Stat


- Nos muestra de forma resumida las modificaciones que se han realizado en  los diferentes archivos en el que se quieren ver las modificaciones.

```git diff –-numstat``` ( solo para ver los números de líneas añadidas y eliminadas)

---

## :star: Pasos a trabajar con los comandos vistos en la case 2 y 3 de Git:

```
Paso 1: Creamos una subcarpeta en la carpeta tecnicatura_git.

Tecnicatura Git:
  Java
  Python
  Readme

En la terminal Git Bash:
 > cd tecnicatura_git
 > mkdir readme

Paso 2: Abrimos cualquier editor de texto que tengan

- Creamos un documento, escribimos unas líneas y lo guardamos en la subcarpeta Readme.

Paso 3: En la terminal de Bash  tecleamos > git status

Paso 4: Agregamos archivos a nuestra área de preparación > git add .

Paso 5:  commiteamos el archivo que ya está en nuestra área de preparación > git commit – m “escribimos nuestra primara línea del documento”, damos enter.

Paso 6: volvemos a nuestro editor de texto y escribimos una 2da. línea y guardamos. (Importante que no se olviden).

Paso 7: En la terminal de Git Bash tecleamos > git status

Paso 8: pasamos modificaciones a nuestra área de preparación y commiteados al mismo tiempo (éste comando sólo se puede utilizar sobre carpetas que ya existen no nuevas).

> git commit –am “ actualizamos notas”

Volvemos al editor de texto y agregamos 3 líneas más

Paso 9: desde la terminal de Git bash eliminaremos esas últimas modificaciones en nuestro editor de texto.

>   git checkout  nombre del archivo

> git checkout  -f si hemos modificado más de un archivo borrará todas las modificaciones realizadas.

Paso 10: Volvemos a nuestro editor de texto “escribimos nuevamente” y guardamos.

Paso 11: Tecleamos :
>git add .
> git restore --staged  nombre del archivo

->Vuelve mi archivo al área de trabajo

Paso 12: Volvemos al editor y agregamos otras líneas, guardamos en nuestra terminal Git Bash tecleamos > git status

Paso 13: Seguimos en nuestra terminal y tecleamos

> git diff 'nombre del archivo en el que estamos  modificando'

> git diff --stat -> me devuelve las últimas modificaciones pero en forma de resumen.

> git diff  --numstat -> solo devuelve número de inserciones y eliminaciones.


---


## : star: Actividad Clase 3 ( 1ra. parte)


### Actividad n°1:

Responder cuestionario de la  Clase 3 n° 1 en el aula del Campus


### Actividad n°2:

- Creamos una nueva carpeta readme

- Abrimos editor de texto

- Trabajamos con los comandos desde la terminal Git 

- Actividad Clase 3 (2da. parte)


### Actividad n°3:

Responder cuestionario n°2 de la Clase n°3 en el aula del Campus.


### Actividad n°4: 

Añadir los archivos modificados aplicando los comando que vimos en la clase de hoy.

---
---

# :book:  Cuarta clase : 03 Mayo - GIT

---

-> [Enlace Documentación Comando Git Log](https://git-scm.com/docs/git-log)


---

## Comandos GIT ya vistos:

```
git commit –am « nota de nuestro cambio»
git checkout «nombre de archivo»
git checkout –f
git restore --staged «nombre de archivo»
git diff
git diff --stat
git diff --numstat
```

-> Cada commit que realizamos irá formando una línea del tiempo
en nuestro proyecto

``` MAIN/MASTER X------X-----X-----X ```

---

## ¿Cómo viajamos en el tiempo para ver los cambios que realizamos en nuestro proyecto?

Cada commit tiene un número de id o #

Otras funciones de **git checkout** -> Con ``` git checkout «más el número de identificación»```(se pueden copiar sólo los primeros 7 dígitos) podremos ver entonces a como estaba nuestro proyecto sin las modificaciones nuevas

Para volver al presente donde esta mi último commit ejecutamos -> ``` git checkout master```

---

Con el comando ``` git log``` se ven los commits hasta el momento

---


- Para utilizar el comando Git Checkout y el nª hash # de cada commit seleccionaremos, cualquier commit que hemos realizado

- Una vez seleccionado lo copiaremos

- Teclearemos el comando ```git checkout <mas el numero hash# de nuestro commit>``` y nos aparecerá una leyenda diciendo que nuestro puntero o posicionamiento cambia del ultimo commit al commit que le hemos indicado con el nª hash#

- Nos indica que nuestro puntero ya esta ubicado en en el numero del commit que seleccionamos y con la descripción del commit que realizamos

- volvemos a teclear ```git log --oneline``` y nos aparecerán los commit sólo hasta el commit
que seleccionamos, los demás commit mas nuevos no aparecerán. Volvemos a seleccionar un commit pero esta vez sólo los primeros 7 dígitos, copiamos y volvemos a ejecutar

- Tecleamos``` git log``` y nos aparecerán sólo hasta el commit que hemos seleccionado, los más recientes no aparecerán.

- El puntero se posicionará en el commit que hemos seleccionado

- Para volver al último commit que realicé tecleamos ```git ckeckout master```

- y el puntero nos vuelve a posicionar en neutro último commit



---

## :star: git log --raw

- Este comando nos permite saber cuales fueron los cambios que pasaron en un commit. 

- Nos mostrará también que tipo de acciones hicimos si modificamos un archivo, lo borramos o añadimos algo nuevo. Además nos muestra el código de seguridad de nuestros commit.


---

## :star: git log

```git log --oneline``` -> este Comando nos permite ver en una hilera un resumen de los hash #
acortados de los cambios que se realizaron en cada commit.


- Nos aparecerá la última rama trabajada porque se respeta siempre el tiempo.

- Podemos observar en la captura la ultima rama creada, mas los commit realizados en la Master


```git log --oneline -n <x>``` -> con este comendo voy a poder ver la cantidad de commit que
quiero leer

- Con este comando voy a poder ver la cantidad de commit que quiero leer.


```git log --pritty=format:<<>>``` ->  este comando permite agregar el formato que se desee,
por ej: el nombre del autor, correo, fecha, etc.

- Ejemplo: ```git log --pretty=format:"El autor del commit %h fue %an" ```


---

El comando Git log es nuestra línea de tiempo.

Esa línea la llamaremos MASTER y siempre se actualizará hacia arriba.

---

## :star: RAMAS

Dentro de mi rama MASTER puedo crear ramas nuevas o auxiliares.

Esto nos indicará que vamos a tener dos líneas de tiempo con diferentes tiempos y commit

```
                  --- X ----- X Nueva rama 1
                  |
Master  X ---- X ----- X ------ X ------ X
o Main                     |
                           ---- X ---- X Nueva rama 2
```


Cada línea tiene su independencia y nuevas características, esto nos permite solucionar problemas que pueden surgir en la Master ý así evitar dañar nuestro proyecto.

```
MASTER X ----- X ------ X ------ X ------ X
         |
         ---- X ---- X DEVELOP
```


Las Ramas nos permiten fusionar más adelante y se pueden generar más líneas 


```
MASTER X ----- X ------ X ------ X ------ X
         |
         ---- X ---- X ---- X DEVELOP
                 |
                 ---- X ---- FEATURE1
```

---

Cada línea del tiempo se llamarán ramas como si fuera un árbol.

-  ```git log``` nos dará la ubicación de nuestra rama Master

- ```git log --online``` nos indicará que estamos en el Master

- ```git log –checkout <el numero de ID del commit>``` nos dará la ubicación especifica de nuestro commit.

-  Si queremos volver a la rama Master ejecutamos el comando ```git checkout master```


---

## :star: RAMA NUEVA


Para Crear una Rama Nueva utilizaremos el siguiente comando -> ```git checkout -b <nombre de la rama>```


En el momento de crear mi **rama auxiliar** o **nueva rama** mi puntero se va a posicionar en mi nueva rama de mi proyecto.

Una vez creada la rama, añadiremos las modificaciones a nuestro proyecto, cuando ya estén listas nuestras modificaciones.

Digitaremos ```git status``` y veremos entonces cada una de las modificaciones que hemos
realizado.

Luego commitearemos dichas modificaciones.

```git add . ```(agregamos archivo modificado)

```git checkout -b <nombre de la nueva rama>```

```git branch``` ( veremos tanto la rama Master como nuestra rama Creada )

---

## git brach


```git branch``` ->  Eeste comando nos permite ver todas las ramas que tenemos tanto nuestra rama Master como todas las creadas.


---

## git log --oneline --all --graph

```git log --oneline --all --graph ``` -> este comando nos va a permitir ver todas las ramas en línea y con los commit (puntos)en cada rama

---

## git log --oneline --all --graph --decorate


```git log --oneline --all --graph --decorate  ``` ->  este comando nos permite ver de manera gráfica (dibujo)de las ramas que se van trabajando por separado y las modificaciones que vamos registrando.


---

## Actividad

**Actividad n°1 (Clase n°4)**: Responder cuestionario para asistencia

**Actividad n°2 (clase n° 4)**:

- 1- Creamos carpeta desde Git Bash «Practica»

- 2-Añadimos un archivo Readme y realizamos modificaciones en el.

- 3- utilizamos comandos ```git checkout``` y ```git log```

**Actividad n° 3(clase4)**:

Creamos una rama nueva con el nombre «Práctica» 

Aplicamos los comandos git log vistos en la clase

Seguir los pasos que están en el aula del campus

---
---
