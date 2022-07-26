# core-code-from-scratch-readme
## Week 1
***Tuesday***
[19/07/2022](WEEK1/Tuesday/README.md)

1. ### Interpreted And Compiled Programming Languages
The programas are instruccions that works to generate some accion. The funcionts of interpreted and compilad languages are to use 
Los programas son instrucciones que sirven para generar una acción. Los lenguajes Interpretados y Compilados tienen como función el usar el código legible para el ser humano para transformarlo en código entendible para la máquina.
| Interpretado | Compilado |
| ------------- | ------------- |
| Se da una copia pero se debe contar con algun intermedio  | Se corre el programa inmediatamente sin tener el código fuente |
| Son más lentos  | Como necesita de que cada instrucción sea traducida, es más eficiente  |
| El código fuente es público | El código fuente es privado |
| Necesita de un programa que entienda el código en tiempo real para ser ejecutado |  Convierte el códgio binario que lee la máquina|
|Ejecutan el programa línea por línea|Deben "reconstruir" el programa cada vez que se haga un cambio|
|Ejemplos: PHP, Python, Javascript|C, C++, Rust|

**OJO:** Cabe resaltar que algunos programas pueden tener implementaciones tanto interpretado como compilado.

2. ### Is Java compiled or interpreted, or both?
Java implementations typically use a two-step compilation process. Java source code is compiled down to bytecode by the Java compiler. The bytecode is executed by a Java Virtual Machine (JVM). Modern JVMs use a technique called Just-in-Time (JIT) compilation to compile the bytecode to native instructions understood by hardware CPU on the fly at runtime.

3. ### Pseudocode Currency Converter
*Pasos para entender el algoritmo*
- Ingrese una cantidad de dinero que desea convertir a bitcoin 
- Guardado de dato
- Usar la conversión de USD a BTC (1 USD = 0,00004467 BTC)
- Mostrar resultado 

*Pseudocode*
- START
- USD <-- GET
- BTC <-- USD* 0,00004467 (23/07/2022)
- PRINT BTC 
- END


4. ### High and Low level languages

| Alto | Bajo |
| ------------- | ------------- |
| Se refiere a lenguaje humano |  Se refiere a lenguaje de máquina|
|Es utilizado en programación|No hay relación con los conceptos de programación|
|Necesita de algún lenguaje interpretado o compilado|Directamente ejecutados en la máquina, sin lenguaje interpretado o compilado|
|Fácil para utilizar|Muy complejo para utilizar|
|Ejemplo: C#, Java, PHP|Ejemplo: Ensamblador |
***Miércoles***
[20/07/2022](WEEK1/MIERCOLES/README.md)
1. ### Your date of birth in the matrix?

- Tener tabla de exponenciales de 2 [tabla](https://todofisico.es.tl/numeracion-binaria.htm)
- Se necesita el año 1999
- Se resta en la tabla comenzando desde 1024 - 1999
- Se llena la tabla usando las restas necesarias

| 1024 | 512 | 256 | 128 | 64  | 32  | 16  | 8   | 4   | 2   | 1   |
| ---- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 1    | 1   | 1   | 1   | 1   | 0   | 0   | 1   | 1   | 1   | 1   |

**Respuesta: 11111001111**

2. ### MIPS
-Mi nombre
![](../assets/00_MIPS.png)
```assembly
  .data
        message: .asciiz "\nMónica\n"
  .text
        main:
              li $v0, 4
              la $a0, message
              syscall
``` 
-numeros
```assembly
.data
	      n1: .asciiz "\nIngrese el primer numero: "
	      n2: .asciiz "\nIngrese el segundo numero: "
  .text
	      main:
          #Input number 1
              li $v0, 4
              la $a0, n1
              syscall

              li $v0, 5
              syscall
        #Save number 1
              move $t0, $v0

        #Input number 2
              li $v0, 4
              la $a0, n2
              syscall

              li $v0, 5
              syscall
        #Save number 1
              move $t1, $v0
        #Print numbers
              li $v0, 1
              move $a0, $t0
              syscall
``` 
***Jueves***
1. ### Print special numbers
- For
- While
- do While
- Even number
- Reminder Operator
2. ### Bad Code
The error is missing a = to be a equality operator ( == ) checks whether its two operands are equal, returning a Boolean result. 

```javascript
var cond = false;

if ((cond == true)){
console.log('The cond variable is true');
}else {
  console.log('The cond variable is false');
}
```
3. ### Bad Code 2
The erros are the use of else if and connect the two conditional with and gate.
```javascript
var n = 100;

if (n == 100) {
  console.log('This is a special number!');
} else if (n < 1000 && n % 10 == 0 ) {
  console.log('This number is almost special');
} else {
   console.log('Just a regular number');
}
```
4. ### Follow Git Course
I'm already started 