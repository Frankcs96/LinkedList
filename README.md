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

# Ventajas de la LinkedList con respecto a un ArrayList

El principal beneficio de las listas enlazadas respecto a los vectores convencionales es que el orden de los elementos enlazados puede ser diferente al orden de almacenamiento en la memoria o el disco, permitiendo que el orden de recorrido de la lista sea diferente al de almacenamiento.

En la siguiente tabla podemos ver el tiempo de ejecución de los arrays y las linkedList en comparativa:

![Onotation](https://i.gyazo.com/7d05140d70acfef31fd1e259b9150ebc.png)


# Clase LinkedList en java

Por suerte java nos trae la implementación de la lista enlazada ya hecha.
![Jerarquia](https://i.gyazo.com/e686557f7f69a9ac1a0148763ba2a896.png)


Sencillo ejemplo de como usar una LinkedList en java:

```java
import java.util.*;
public class AnimalesEnlazados{
   public static void main(String args[]){

     LinkedList<String> animales =new LinkedList<String>();

     //Añadir elementos a la lista
     animales.add("Perro");
     animales.add("Gato");
     animales.add("Ratón");

     //Añadir elemento a la primera posición
     animales.addFirst("Zebra");

     //Añadir elemento a la ultima posición
     animales.addLast("León");

     //Añadir elemento a una posición determinada
     animales.add(2, "Caballo");

     //Iterar sobre una LinkedList
     Iterator<String> iterator = animales.iterator();
     while(iterator.hasNext()){
       System.out.println(iterator.next());
     }
   } 
} 


```
# Métodos mas comunes de la clase LinkedList

* **add(elemento)** -> Añade un elemento a la ultima posicíon de la lista

* **addFirst(elemento)** -> Añade un elemento a la primera posicíon de la lista

* **addLast(elemento)** -> Añade un elemento a la ultima posicíon de la lista

* **clear()** -> Deja la lista vacia

* **add(elemento)** -> Añade un elemento a la ultima posicíon de la lista

* **get(index)** -> Nos devuelve el valor de cierta posición en la lista

Para mas información sobre como funciona la clase consultar la API de java https://docs.oracle.com/javase/8/docs/api/java/util/LinkedList.html
