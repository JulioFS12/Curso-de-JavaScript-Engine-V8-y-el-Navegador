# Curso-de-JavaScript-Engine-V8-y-el-Navegador

[Evolucion de la web](http://www.evolutionoftheweb.com/)

### Historia JavaScript

* Mocha : 1995
* LiveScript: 1995
* JavaScript: 1995
* JScript: 1995
* EcmaScript: 1997
* V8: 2008
* Nodejs: 2009
* Frameworks: 2010
* ES: 2016

###  EcmaScript
ECMAScript es el lenguaje de scripting que forma la base de JavaScript. ECMAScript está estandarizado por la organización de estándares ECMA Internacional en las especificaciones ECMA-262 y ECMA-402. [more...](https://developer.mozilla.org/es/docs/Web/JavaScript/Language_Resources)

### JavaScript Engine

Los motores son esas programas que se encargan de convertir código de alto nivel (JavaScript, Python, C) a código de bajo nivel (Machine Code, Bytecode). Cada navegador tiene su propio motor para compilar e interpretar JavaScript.

### Compilador
El compilador es el programa encargado de convertir código escrito en un lenguaje de programación a otro lenguaje de programación de bajo nivel. Por ejemplo, el compilador del V8 es el encargado de transformar JavaScript a Bytecode y luego a Machine Code.

### Interprete

El intérprete es el encargado de revisar el código línea por línea y ejecutarlo directamente en la máquina de destino. Cabe resaltar que los intérpretes también realizan algún trabajo de traducción al igual que los compiladores.

![imagen](https://res.cloudinary.com/practicaldev/image/fetch/s--Xs5OQmGX--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_66%2Cw_880/https://thepracticaldev.s3.amazonaws.com/i/pv4y4w0doztvmp8ei0ki.gif)

![imagen](https://res.cloudinary.com/practicaldev/image/fetch/s--ID8wDIAy--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_66%2Cw_880/https://thepracticaldev.s3.amazonaws.com/i/bic727jhzu0i8uep8v0k.gif)

![imagen](https://res.cloudinary.com/practicaldev/image/fetch/s--6IHw1BUH--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_66%2Cw_880/https://thepracticaldev.s3.amazonaws.com/i/sgr7ih6t7zm2ek28rtg6.gif)

![imagen](https://res.cloudinary.com/practicaldev/image/fetch/s--HlXdsZRx--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_66%2Cw_880/https://thepracticaldev.s3.amazonaws.com/i/i5f0vmcjnkhireehicyn.gif)

### Hoisting

El hosting nos ayuda a comprender el codigo que hacemos, 

* Si llamamos una variable antes de ser declarada, el compiler crea la variable en la memory heap y la inicializa como undefined
* En el caso de las funciones es distinto, primero mandamos a llamar a las funciones antes de ejecutarlas y cuando el interprete la encuentre la ejecuta.
* El hoisting a veces funciona pero no tenemos control de las variables que se van a cambiar
* Si llamamos a una constante (const) antes de inicializar retorna un error de tipo: Uncaught ReferenceError, que corresponde a variables que son referenciadas pero no pudieron * ser capturadas

### Heap Memory

El memory heap es el espacio en memoria donde se guardan todas las funciones, variables, objetos, arrays del código, como objetos de forma no lineal e independiente, creando una referencia a ese dato al cual con dicha referencia luego se puede acceder al contenido de forma más sencilla.

### Call Stack

La pila de llamadas, “call stack”, es una estructura dinámica de datos LIFO que almacena información sobre las subrutinas de una aplicación. Piensalo como el lugar para llamadas de funciones, o una estructura de datos que implementa el tipo de datos de la pila (stack), es el lugar donde se llaman las funciones o procesos de una aplicacion donde solamente se puede ejecutar una función a la vez.

### Garbage Collection
Limpia la memoria de los datos no utilizados para no sobrecargarla y seguir trabajando sin problemas, en otras palabras cuando dejamos de usar el valor que tiene una variable y lo elimina cuando le asignamos otro valor.

![Imgane](https://i.stack.imgur.com/shG8h.gif)

