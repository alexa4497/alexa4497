Universidad de Antioquia 
Desafio 1 - Pre Informe 
Estudiantes: Alexa Carolina Gamboa Mier y Manuela Arboleda Montoya
Semestre: 2025/2
informatica 2

1. Análisis del problema y consideraciones para la alternativa de solución propuesta  

Después de analizar el problema llegamos a las siguientes conclusiones, el usuario debe ingresar el mensaje encriptado y un fragmento del mensaje desencriptado (texto plano), exclusivamente el mensaje que tenga el cliente debe estar comprimido por RLE o LZ78.

Para aplicar el proceso de desencriptado el mensaje que brinda el usuario debe estar previamente encriptado utilizando rotación de bits, no se tiene en cuenta otro tipo de algoritmo para desencriptar. 
 
Es importante mencionar que el codigo no puede tener variables que en lo posible trabajen con datos tipo string, ademas el mensaje encriptado debe tener numeros enteros del 0 al 9, letras de la A a la Z, tanto mayusculas como minisculas, excluyendo signos de puntuacion, tildes y sin la Ñ, por eso es necesario crear un algoritmo para validar que el codigo encriptado que tiene el usuario si cumpla con los requisitos.

2. Algoritmos implementados

Para cubrir las necesidades de los clientes es necesario desarrollar los algoritmos suficientes para el proceso de desencriptado, compresión y descompresión utilizando los métodos brindados, hasta el momento tenemos pensado crear 6 algoritmos, uno que identifique el tipo de proceso de compresión, un algoritmo para el proceso LZ78, uno para RLE, otro algoritmo para todo el proceso de desencriptado usando rotación de bits,un algoritmo que nos ayude a validar que los valores de entrada sean admitidos por el programa y convierte los caracteres en variables de tipo int y asi evitar usar variables de tipo string y por ultimo un algoritmo para verificar que el mensaje desencriptado resultante coincida con el fragmento de mensaje que el cliente tiene. 

3. Tareas definidas para el desarrollo de los algoritmos

Tuvimos en cuenta diferentes tareas que necesitan aplicar los algoritmos para su funcionamiento, son las siguientes:

	-- Algoritmo 1: RLE --

	Tarea 1: Recorrido secuencial, la primera tarea leerá los caracteres uno a uno.
	Tarea 2: Cuenta las repeticiones es decir cuántas veces aparece repetida una letra.
	Tarea 3: Agrupa el número de veces que se repite (signo) y lo asocia con la letra.
	Tarea 4: Indicarle algoritmo se repite hasta que termine la secuencia.  

	-- Algoritmo 2: LZ78 --

	Tarea 1: Reducir la redundancia de un texto reemplazando repeticiones por referencias mas cortas
	Tarea 2: Guardar la misma secuencia varias veces.
	Tarea 3: Se usa un diccionario dinamico para comprimir.
	Tarea 4: Se recibe la secuencia de pares y reconstruye el texto original creando el mismo diccionario que uso el el compresor.

	-- Algoritmo 3: Identificar el tipo de descompresión --

	Tarea 1: El algoritmo debe de recorrer el mensaje que brinda el usuario 
	Tarea 2: identificar el tipo de compresión dependiendo del patrón del mensaje encriptado, se le aplicaran condicionales que evalúen la estructura del mensaje y así llegar a el método de descompresión adecuado.
	Tarea 3: Para evitar errores en cuanto a la seleccion de el metodo de descopresion adecuado el programa estrictamente debe probar con metodo RLE o LZ78. 
	
	-- Algoritmo 4: Validacion de entradas y conversion de str --

	Tarea 1: Verifica que los caracteres de entrada sean o numeros enteros del 0 al 9 , o letas de la A a la Z ,excluyendo la ñ.
	Tarea 2: Como el programa no puede contener variables de tipo str alternamos usando la tabla asci para darle a cada caracter el valor correspondiente.

	-- Algoritmo 5: Desencriptado con rotación de bits y operación XOR --

	Tarea 1: El algoritmo debe aplicar la operación XOR con el mensaje encriptado en binario con la clave en binario 
	Tarea 2: Con el resultado anterior el programa tendrá que aplicar un proceso de rotación de bits dependiendo de la condición (rotación hacia la derecha u izquierda)

	-- Algoritmo 6: Verificación con fragmento de texto plano --

	Tarea 1: Tiene dos valores de entrada , el mesaje desencriptado y el el texto plano que brinda el cliente.
	Tarea 2: Se hace una compracion entre estos dos y si el texto plano coincide con algun fragmento del mensaje entonces el proceso de desencriptado y descompresion fue exitoso.

4. Problemas afrontados en el desarrollo 

Cuando comenzamos el proceso de desarrollo del desafío enfrentamos problemas conceptuales, ya que no entendíamos el proceso de compresión LZ78, también dificultades cuando se hace el proceso de desencriptado usando rotación de bits. 

