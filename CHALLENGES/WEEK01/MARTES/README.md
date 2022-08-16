1. ### Interpreted And Compiled Programming Languages

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
*Steps to undestand the algorithm *
- Enter an amount of money to convert to bitcoin  
- Save data
- Use the conversion to USD to BTC (1 USD = 0,00004467 BTC)
- Show the result 
 

*Pseudocode*
- START
- USD <-- GET
- BTC <-- USD* 0,00004467 (23/07/2022)
- PRINT BTC 
- END


4. ### High and Low level languages

| High | Low |
| ------------- | ------------- |
| Refers to human language |  Refers to machine language|
|It's use in programming|No related to programming concepts|
|Needs an Interpreted And Compiled Programming Languages|Directly executed by the machine, without  an Interpreted And Compiled Programming Languages |
|Easy to use| Very difficult to use|
|Example: C#, Java, PHP|Example: Assembly |