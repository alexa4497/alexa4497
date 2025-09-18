Universidad de antioquia 
Desafio 1 - pre informe 
Estudiantes: Alexa carolina gamboa mier y Manuela Arboleda montoya
semestre: 2025/2
informatica 2


1. Análisis del problema y consideraciones para la alternativa de solución propuesta.  

Después de analizar el problema llegamos a las siguientes conclusiones , el usuario debe ingresar el mensaje encriptado y un fragmento del mensaje desencriptado (texto plano) , exclusivamente el mensaje que tenga el cliente debe estar comprimido por RLE o lempel-ziv.

Para aplicar el proceso de desencriptado el mensaje que brinda el usuario debe estar previamente encriptado utilizando rotación de bits , no se tiene en cuenta otro tipo de algoritmo para desencriptar.

2. Algoritmos implementados

Para cubrir las necesidades de los clientes es necesario desarrollar los algoritmos suficientes para el proceso de desencriptado, compresión y descompresión utilizando los métodos brindados, hasta el momento tenemos pensado crear 6 algoritmos, uno que identifique el tipo de proceso de compresión, un algoritmo para el proceso LZ78, uno para RLE , otro algoritmo para todo el proceso de desencriptado usando rotación de bits,un algoritmo que nos ayude a validar que los valores de entrada sean admitidos por el programa y convierte los caracteres en variables de tipo int y asi evitar usar variables de tipo str y por último un algoritmo para verificar que el mensaje desencriptado resultante coincida con el fragmento de mensaje que el cliente tiene 

3.  tareas definidas para el desarrollo de los algoritmos

tuvimos en cuenta diferentes tareas que necesitan aplicar los algoritmos para su funcionamiento, son las siguientes:

	-- Algoritmo 1 : RLE --

	tarea 1 : recorrido secuencial, la primera tarea leerá los caracteres uno a uno  
	tarea 2: Cuenta las repeticiones es decir cuántas veces aparece repetida una letra.
	tarea 3: Agrupa el número de veces que se repite (signo) y lo asocia con la letra .
	tarea 4 : Indicarle algoritmo se repite hasta que termine la secuencia  

	-- Algoritmo 2: LZ78 --

	-- Algoritmo 3 : Identificar el tipo de descompresión --

	tarea 1 : El algoritmo debe de recorrer el mensaje que brinda el usuario 
	tarea 2 : identificar el tipo de compresión dependiendo del patrón del mensaje encriptado , se le aplicaran condicionales que evalúen la estructura del mensaje y así llegar a el método de descompresión adecuado.
	tarea 3: Para evitar errores en cuanto a la seleccion de el metodo de descopresion adecuado el programa estrictamente debe probar con metodo RLE o LZ78. 
	
	-- Algoritmo 4 : validacion de entradas y conversion de str --

	tarea 1:Verifica que los caracteres de entrada sean o numeros enteros del 0 al 9 , o letas de la A a la Z ,excluyendo la ñ.
	tarea 2:Como el programa no puede contener variables de tipo str alternamos usando la tabla asci para darle a cada caracter el valor correspondiente.

	-- Algoritmo 5 : desencriptado con rotación de bits y operación XOR --

	tarea 1: El algoritmo debe aplicar la operación XOR con el mensaje encriptado en binario con la clave  en binario 
	tarea  2: Con el resultado anterior el programa tendrá que aplicar un proceso de rotación de bits dependiendo de la condición (rotación hacia la derecha u izquierda)

	-- Algoritmo 6: verificación con  fragmento de texto plano --

	tarea 1:Tiene dos valores de entrada , el mesaje desencriptado y el el texto plano que brinda el cliente.
	tarea 2:se hace una compracion entre estos dos y si el texto plano coincide con algun fragmento del mensaje entonces el proceso de desencriptado y descompresion fue exitoso.

4. Problemas afrontados en el desarrollo 

Cuando comenzamos el proceso de desarrollo del desafío enfrentamos problemas conceptuales, ya que no entendíamos el proceso de compresión LZ78, también dificultades cuando se hace el proceso de desencriptado usando rotación de bits. 

