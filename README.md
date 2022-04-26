# TiposDeDatosEnJava

##JVM (Java Virtual Machine)
![RAM](ram.jpeg)
* Realiza una gestion eficiente de la memoria.
* Distribuye la memoria en dos zonas: Stack (Pila) y Heap (Monton).

###Stack
* Se almacenan: Varaibles locales, llamadas a metodos (parametros y resultados) , variables primitivas, referencias a obejtos del heap.
* Memoria estatica.

###Heap
* Es gestionado por el Garbage Collector
* Espacio de memoria en timepo de ejecucion donde se registran los objetos.
* Memoria dinamica.
* No posee estructura de asignacion de espacios.

### Variable
* Contenedor de memoria donde se almacena informacion.
* En Java se desclara con un tipo que se conservara durante todo su ciclo de vida en el interior de la aplicacion.
* La variable debe de tener un nombre.
* Existen te tipo Primitivo y Referenciado.

## PRIMITIVOS 
* Contenedores de tamaño especifico que almancenan valores y no tienen metodos.
* Ejemplos: boolean, char, byte, short, long, float, double.

## REFERENCIADOS
* Almacenan las referencias a los datos.
* Estos datos se escriben en una zona de memoria llamada heap.
* Espacio de memoria en tiempo de ejecucion donde se registran los objetos.
* Accesible dede otras instancias de clase.
* Su ciclo de vida termina cuando no necesita mas.
* Mientras exista al menos una referencia activa en la zona de datos esta se mantendra.
* Tan pronto como no haya mas referencias, la zona se considera no utilizada y preocede a su destruccion por parte del Garbage Collector.
* Un tipo referenciado puede no referenciar nada -> null
* new : instanciacion de una clase. Reserva una direccion de un area de memoria.

### Variable de referencia 
* Caracteriza una instancia de clase, es decir la direccion  de donde esta el objeto.
* Contiene la direccion de un objeto, cuyo valor por defecto es null.
* Durante una prueba e igualdad entre dos variables por refencia, sin las direcciones de los objetos lo que se compara, y no el contenido de los objetos en si mismos.
* Cuando se usa una referencia como argumento de un metodo es la direccion del objeto lo que se pasa, y no el objeto en si mismo.