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