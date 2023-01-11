# Notas de programacion
## **Nombre:** Gabriel Del Valle 
___ 

# **Bloque 1**

## **Introduccion a la programacion.**
___
### ***Atajos de teclado o shortcuts***
Se repasaron los distintos atajos y se uso la "chuleta" para aprenderlos de mejor manera.

![Chuleta](/Imagenes%20Md/chuleta.png)
___
### ***Uso del git y git hub***

Se revisaron todos los codigos para el uso correcto del git.
Como principal usamos el "**git init**":

Posteriormente se usa:
- gitinit
- gitstatus
- gitadd.
- gitaddNombreCarpeta/NombreArchivo
- gitcommit-m 'mensaje : initialprojectversion

Para crear una carperta que ignore los archivos que no son de utilidad se usa:
- echonombreArchivo.ext>>.gitignore 
- echo*.txt>>.gitignoregi
___

### ***Programación estruturada***

El curso se inicio con el Lenguaje C.

Primero aprendimos los tipos de datos por ejemplo:

- **int** : números enteros.
- **float** : números decimales.
- **char** : un caracter.

Existen muchas más.

Tambia se aprendio los tipos de control de flujo por ejemplo:

- **if-else** : Condicional.
- **for()** : tipo de bucle.
- **while** : bucle (este primero mira la condicion y luego ejecuta).
- **do while** : Otro bucle (primero ejecuta y luego mira la condición).
- **swich** : genera varios casos.

___
### ***Algoritmia***

La algoritmia se usa para encontrar soluciones a problemas mediante una serie de pasos

1. Pseudocodigo.
2. Diagrama de flujo. 
3. Codificacion del programa.
4. trace(seguimiento).

**Ejemplo diagrama de flujo:**

![Diagrama](/Imagenes%20Md/Ejemplo%20diagrama.png)


___
### ***Introduccion general***

El lenguaje C permite realizar programacion estructurada de forma sencilla ya que economiza expresiones con abundancia de operadores y tipos de datos.
La libreria que usamos en C es el stdio.h y tenemos las funciones  y procedimientos por ejemplo el **int** que es una funcion ya que retorna datos o el **void** que es un precedimiento ya que no retorna nada.

Tambien se aprendio como se declaran variables y su inicialización por ejemplo.
 ~~~
 int a = 2:
 int b = 3;
 char a = 'b';
~~~
___
###  ***Estructura de control***

Para esto tenemos que inicializar la funcion o precedimiento con un nombre que nos diga lo que hace esa funcion o precedimientos por ejemplo.
~~~
int showSuma(){
}
~~~
Como dice el nombre esta funcion seria para mostrar y resolver dumsd.

~~~
void showNombres(){

}
~~~

Lo que se supone que haria esta es mostrar nombres.
___

### ***Operador ternario***

Se usa para saber si un dato es multiplo de dos, esto nos da una gran variedad de utilidades por ejemplo imprimir solo letras pares o numeros pares.

~~~
if ((j+i)%2 == 0){
    printf("+ ");
}
else{
     printf("- ");  
}
~~~
___
 ### ***Serializacion de datos***

 Nos permite indicar el tipo de dato que se esta usando ya que al ingresar otro tipo de dato nos da un error.
 Por ejemplo:
 ~~~
printf("\nchar%c",c );
 ~~~
Nos indica que estamos usando un caracter .

___

### ***Procedimientos y funciones***
 La diferencia radica en que los procedimientos **no retornan** ningun valor ni dato mientras que las funcionas **si retornar** valores o datos.

Ejemplo procedimiento:
~~~
voidshowConsola(intrta){
    printf("La suma es: %i\n", rta);
}
~~~
Ejemplo función:
~~~
intsumaInt(inta, intb){
    returna+b;
}
~~~
___

### ***Arrays***

Los arrays son variables estructuradas, donde cada elemento se almacena de forma
consecutiva en memoria. Ademas se los gurada inicializando el tipo de dato + nombre[i]; donde i es el numero de espacios que puede tener el array. Por ejemplo:

~~~
int main(){

    char nombre[6];
    char nombre[] ={'G','a','b','r','i','e','l'};
    char nombre[]="Gabriel";
}
~~~
En el ejemplo anterior se indica las distintas formas de guardar un arrays donde ken numero en el interior de los corchetes representa el espacio del mismo.

Ejemplo uso de array:
~~~
void validaClave()
{
   char clave[10];
   printf("Escriba su clave: ");
   scanf("%9s", clave); 

   if (strcmp(clave, "itsa")==0){
      printf("La clave es correcta");
   }
   else{
      printf("La clave es incorrecta");
   }
}
~~~
___

### ***Arrays en dos dimensiones o Matrices***

Matrices o tambien conocidos como arrays en dos dimensiones, funcionan como un array normal con la diferencia de que se inicializan nombre[i][j] donde i y j representan el numero de filas y columnas.

Ejemplo de matriz:
~~~
void matrizInteger()
{
    int edades[3][2] = {{1,2},{9,8},{14,21}};
    int filas = (sizeof(edades)/sizeof(edades[0]));
    int columnas = (sizeof(edades[0])/sizeof(edades[0][0]));

    system("clear");
    printf("filas: %i \n",filas);
    printf("columnas: %i \n",columnas);
    for (int i = 0; i < filas; i++)
    {
        for (int j = 0; j < columnas; j++)
        {
            printf("%i \t",edades[i][j]);
        }
        printf("\n");
    }
    system("pause");
}
~~~
___

### ***Estructuras y uniones***

Las estructuras contienen varios datos y se la define usando la palabra "**struct**".
~~~
 struct mystruct
{int int_member;
double double_member;
char string_member[25];    
}variable;
~~~
___

### ***Enumeradores***

El enumerador es una constante de un numero entero, sirve para crear listas de tipos de datos que se asocias a constantes.

Ejemplo de como definir un enumerador:

~~~
 enum
>{
    enumerador1,enumerador2;
};
~~~
___

### ***Archivos y operaciones de archivos***
Mediante el uso de la libreria stdio.h se nos permite crear ficheros para crear carpetas, depositar nuestros archivos, importar datos de un archivo aparte entre mas opciones. Para realizar el uso correcto de estas se usa las siguientes palabras reservadas.

|Nombre|Función|
|------|-------|
|fopen()|Abre un archivo|
|fclose()|Cierra un archivo|
|fgets()|Lee una cadena de un archivo|
|fputs()|Escribe una cadena en un archivo|
|fseek()|Busca un byte específico de un archivo|
|fprintf()|Escribe una salida con formato en el archivo|
|fscanf()|Lee una entrada con formato desde el archivo|
|feof()|Devuelve cierto si se llega al final del archivo|
|ferror()|Devuelve cierto si se produce un error|
|rewind()|Coloca el localizador de posicion del archivo al principio del mismo|
|remove()|Borra un archivo|
|fflush()|Vacía un archivo|
