# Conceptos y Paradigmas de Lenguajes de Programación

### Lenguajes Asignados:
  * C
  * Matlab

#### Grupo 3
  * 14859/2 - Adrogué Benas María Noel
  * \*\*\*\*\*/* - Farinella Robertino


### Referencias

* Primera Parte
  * *The c programming language* - Brian W. Kernighan y Dennis M. Ritchie.
  * *The GNU C Reference Manual*. [link](http://www.gnu.org/software/gnu-c-manual/gnu-c-manual.html)
  * Documentación oficial de Matlab. [link](https://www.mathworks.com/help/matlab/index.html)

*****

# Primera Parte
## A.

>   Enuncie y compare distintos aspectos semánticos (tanto de la semántica estática y dinámica) de cada uno de los lenguajes asignados.

#### Semántica estática

- **Declaración de Variables**

  - C
    En C se deben declarar todas las variables antes de su uso, generalmente al principio de la función y antes de cualquier proposición ejecutable, esto se denomina *tipado estático*. Una variable en C consta de un nombre de tipo, de los cuales C provee muchos, seguido por una lista de variables, por ejemplo:
    ```
      int aux;
    ```

  - Matlab
    Al contrario de C, Matlab utiliza un solo tipo de variable, el arreglo. Este arreglo puede ser unidimensional, como un vector e incluso un valor (en caso de poseer un solo elemento), o multidimensional, como una matriz.
    ```
      A = 5 (matriz unaria de enteros)
      B = ['a' 'b' 'c'] (matriz unidimensional de caracteres)
    ```
    Una variable puede ser declarada sin su tipo y el lenguaje identifica de qué tipo es por los valores de inicialización de la misma, esto se denomina *tipado dinámico*.

- **Asignación y cambio de variables a distintos tipos**

  - C
    En este lenguaje, una variable no puede cambiar de tipo, razón por la cual querer asignar un string a una variable de tipo entero, por ejemplo, generará un error. Uno puede realizar, sin embargo, lo que se denomina un *casting* para poder utilizarla como si fuera de otro tipo. Un *casteo* crea una copia en el tipo indicado de la variable, no modifica la variable original.

  - Matlab
    Por el contrario en Matlab una variable, al ser todos arreglos, puede cambiar de tipo de elemento en cualquier momento. Una matriz unidimensional de enteros puede pasar a ser una matriz multidimensional de caracteres sin ninguna sintaxis particular. No puede, eso si, combinar operaciones de elementos numéricos con otro tipo de elementos o comparar dos arreglos de distintas dimensiones (a no ser que uno sea un arreglo de un elemento, el cual se comporta como un solo valor).

- **Signatura o Firma de una función**

  - C
