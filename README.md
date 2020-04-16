# LinkedList
En este repositorio voy a dar información detallada sobre la LinkedList en concreto de Java
# Concepto

Una lista enlazada es una colección o secuencia de elementos dispuestos uno detrás de otro, en la que cada elemento se conecta al siguiente elemento por un “enlace” o “referencia”. La idea básica consiste en construir una lista cuyos elementos, llamados nodos, se componen de dos partes (campos): la primera parte contiene la información y es, por consiguiente, un valor de un tipo genérico (denominado Dato, TipoElemento, Info, etc.), y la segunda parte es una referencia (denominado enlace o sgte) que apunta (enlaza) al siguiente elemento de la lista.

![Lista](https://sites.google.com/a/espe.edu.ec/programacion-ii/home/listas-enlazadas/lista.png?attredirects=0)

# Tipos de LinkedList

* **Listas simplemente enlazadas:**  Cada nodo (elemento) contiene un único enlace que lo
conecta al nodo siguiente o nodo sucesor. La lista es eficiente en recorridos directos
(“adelante”).

* **Listas doblemente enlazadas:** Cada nodo contiene dos enlaces, uno a su nodo predecesor
y otro a su nodo sucesor. La lista es eficiente tanto en recorrido directo (“adelante”) como
en recorrido inverso (“atrás”).

* **Lista circular simplemente enlazada:** Una lista enlazada simplemente en la que el último
elemento (cola) se enlaza al primer elemento (cabeza) de tal modo que la lista puede ser
recorrida de modo circular (“en anillo”).

* **Lista circular doblemente enlazada:** Una lista doblemente enlazada en la que el último
elemento se enlaza al primer elemento y viceversa. Esta lista se puede recorrer de modo
circular (“en anillo”) tanto en dirección directa (“adelante”) como inversa (“atrás”).
