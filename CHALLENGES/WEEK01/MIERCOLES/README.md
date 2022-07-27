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