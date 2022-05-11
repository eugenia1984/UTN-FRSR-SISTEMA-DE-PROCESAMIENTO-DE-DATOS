# :book: Clase 5: 10 Mayo

---

## :star: Comandos Git y Trabajo Git

### Recordatorio de la clase anterior:


• Git Checkout

• Git log

• Git branch

• Git switch

---
---

## :star: Repaso de algunos Conceptos:

**Commit**:  es un conjunto de cambios en los archivos que hemos  confirmado y que queremos almacenar  para un futuro. Los commits se relacionan unos con otros en una o varias secuencias para poder ir viendo la historia de un determinado archivo a lo largo del tiempo.

```    
          5	4	3	2	1
	  t	t	t	t	t
	  i	i	i	i	i
	  m	m	m	m	m
	  m	m	m	m	m
	  o	o	o	o	o	
MAIN	  C	C	C	C	C
MASTER    *-----*-------*-------*-------*
          |
        HEAD
```

**El concepto de HEAD** : se refiere al commit que está dentro de tu repositorio posicionado en cada momento. Por regla general HEAD suele coincidir con el último commit de la rama en la que estés ubicado, ya que habitualmente estás trabajando en lo último. Pero si te mueves hacia cualquier otro commit anterior entonces el HEAD estará más atrás.

```
HEAD -> X -> COMMIT
```

**Guiones en Git**:  Para entender los comando que estamos aplicando desde **Git Bach** es importante saber el significado.

- **-** (un sólo guión)  acompaña una o dos letras.  Ej: ``` > git checkout -b```


- **--** (dos guiones) acompañan una palabra. Ej: ```> git log --```

«Cuando se hace ``` > git log``` el **HEAD** nos indica en que rama estamos ubicado.»

---

## :star: ¿Cómo hacer para eliminar un commit?


Para poder eliminar un commit utilizaremos el comando: ``` > git reset <hash del commit>```.

Este comando permite eliminar la modificación que commiteamos. -> Nos aparece el commit que eliminamos como el último commit que realizamos.


---

## :star: Ramas (branches)

Existe una rama predeterminada que se crea automáticamente cuando se crea un repositorio que se llama **Rama Master**.

Actualización posterior: hasta mediados del año 2020 esta rama se llamaba**master** y no**main**. Pero por aquel entonces, aunque existen diversas teorías sobre el origen de ese nombre, se decidió que era una referencia al esclavismo ("master" de "amo", frente a "slave" de "esclavo. Otras teorías hablan, de que viene de "master copy" o copia maestra o principal) y que había que renombrarla. Así que ahora es "main" y no "master".

### Nuestra Rama Master hoy llamada Main :

Por regla general a **Main** se la considera la **rama principal** y la **raíz** de la mayoría de las demás ramas. Lo más habitual es que en main se encuentre el **"código definitivo"**, que luego va a producción, y es la rama en la que se mezclan todas las demás tarde o temprano para dar por finalizada una tarea e incorporarla al producto final:

```
                                MASTER/MAIN
                                      |
* ----- * ------- * ------ * -------- * ------- * ------ *
                           |          |         |        |
                             COMMITS          NUEVOS COMMITS
```


En la clase n°4 estuvimos viendo como crear nuevas ramas.

Con el comando: ```> git checkout  -b <nombre de la nueva rama>```

Y con el comando: ``` > git branch``` nos permite ver todas las ramas que tenemos , tanto la rama creada como la rama Master.

Como se puede apreciar en la imagen, se crea una rama auxiliar , se realizan commit en ella y luego se fusiona  nuevamente a la rama principal o rama Master.

```
MASTER  * ---> * -------------------------->*
                |                           |
          BRANCH |                         |
NEW_FEATURE       -------------------------
     
```
---

## :star: ¿Qué es Git Merge?

**Git Merge** es un comando que se usa para fusionar ramas independientes en una sola rama en Git.

Cuando se usa el comando de fusión en Git, solo se actualiza la rama actual para reflejar la fusión y la rama de destino no se ve afectada. Esto significa que, a menudo, Git Merge se usa junto con git checkout para seleccionar la rama actual y git branch para eliminar una rama fuente desactualizada.


-> Git Merge es un comando para fusionar ramas en Git

### ¿Cómo funciona Git Merge?:

El uso principal del comando Git Merge es fusionar dos ramas. También se utiliza para fusionar cadenas de confirmación en un historial unificado.

Para comprender cómo funciona el comando Git Merge, tomaremos un ejemplo de combinación de ramas. En la siguiente ilustración, Git Merge tomará dos ramas y encontrará una confirmación de base común entre ellas. Cuando Git encuentra una confirmación de base común, crea una nueva confirmación de combinación y combina los cambios en la secuencia de cada confirmación de combinación. Aquí, tenemos 2 sucursales: sucursal principal y sucursal de etapa. Ahora, fusionaremos la rama del escenario con la rama principal.


### Cómo fusionar las ramas que hemos creado?

- Utilizarás el comando ```git merge```

- Indicarás haciendo ```git merge <nombre de la rama>``` a la rama cuál querrás fusionar con master.


**«Siempre tener en cuenta que cuando se mezclan ramas se debe tener cuidado con los archivos que se han tocado. Cuando no se tocan los mismos archivos no hay inconvenientes, pero cuando se tocan los mismos archivos git no sabrá cuál archivo agregar y habrá un conflicto.»**


---
---


