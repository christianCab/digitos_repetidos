<!DOCTYPE HTML>
<html>
<head>
    <meta charset="utf-8"/>
    <title>Resolución de problemas y algoritmos</title>
</head>
<body>
    <h1>Problema del TP N°8 </h1>
    <div>
    <h1><b>Ejercicio N°2: </b> Enunciado </h1>
        Un número natural tiene dígitos repetidos cuando alguno de sus dígitos aparece más de una vez.<br>
        Ejemplos:<br>
        Tienen dígitos repetidos 808, 33 y 100.<br>
        No tienen dígitos repetidos 102, 12 y 3<br>
        Implementar un programa que muestre todos los números naturales que tengan dígitos repetidos<br>
        hasta un valor N > 100. El valor N debe ser ingresado por el usuario y validado por el programa.<br>
        El programa debe estar dividido en sub-problemas (funciones:Repetidos y Pertenece; procedimiento: ValidarEntrada)<br>
    </div>
    <div>
        Algoritmo REPETIDOS<br>
        Dato de entrada : num (entero)<br>
        Dato de Salida: REPETIDOS (booleano)<br>
        hay ← falso<br>
        Mientras (num > 0) Y (NO hay) hacer<br>
        <blockquote> dig ← num mod 10</blockquote>
        <blockquote>num ← num div 10 </blockquote>
        <blockquote>hay ← PERTENECE (dig, num) //esta primitiva busca el dígito dig en num </blockquote>
        REPETIDOS ← hay
    </div>
    <div>
        <h1>Funciones y procedimientos del problema (Sub-problemas)</h1>
        <h2>Procedimiento validarDato():</h2>
        <p>
            El el encargado de validar que el numero ingresado por el usuario sea mayor a 100.
        </p>
        <h2>Función pertenece():</h2>
        <p>
            si en un bucle de 0 al numero ingresado por el usuario, se encuentran números naturales con dígitos iguales en el mismo numero, retorna un tipo de dato booleano (true/false).<br>
            -si digito esta en num, mostrar verdadero, el bucle de repetidos ya esta corriendo.
        </p>
        <h2>Función repetidos():</h2>
        <p>
            corrobora en el numero ingresado por el usuario, luego de ser validado, cuenta con más de un digito igual digito parecido.<br>
            -ingresa el numero a descomponer;<br>
            -inicia un bucle capas de descomponer el numero hasta que este sea 0;<br>
        </p>
        <h2>Programa global:</h2>
        <p>
            El usuario ingresa un numero entero (el cual es interrumpido por el procedimiento validarDato); consecutivo a validar el número, el mismo es ingresado en la función repetidos(), donde se descompone el número y se suma la cantidad para controlar, si algún digito se repite mas de una vez.<br>
            Para un hasta el numero ingresado, controlar que, cada iteracion revea si se repite algun digito.<br>
            <h3>Varibles:</h3><br>
            <b>num:</b> es la variable global de tope (entero), ingresada por el usuario, el cual luego pasa por el procedimiento validarDato().<br>
            <b>i:</b>variable iteradora (entero).<br>
            <b>inicio: </b>inicio de la iteracción del programa (entero).<br>
            <b>condicion: </b>variable encargada de almacenar el tipo de dato de salida (booleano), en la llamada a la función repeticion().
        </p>
    </div>
</body>
</html>
