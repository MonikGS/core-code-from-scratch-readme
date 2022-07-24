# core-code-from-scratch-readme
## Week 1
***Tuesday***
[19/07/2022](WEEK1/Tuesday/README.md)


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
-DONE
***Jueves***
1. ### Print special numbers

2. ### Bad Code
3. ### Bad Code 2
4. ### Follow Git Course