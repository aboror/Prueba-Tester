Errores encontrados en el código. 

1) Error: let randomNumber = Math.random() * 100;

Nota: Cuando se crea número aleatorio usando Math, los números son decimales, por lo tanto se hace la conversión a enteros. Quedaría de la siguiente manera.

randomNumber = parseInt(Math.random() * 10);

2) Estaban declarando una variable constante con una valor de 5 que en teoría, es la canttidad de intentos. Que este caso serían 10

Error:   const ATTEMPS = 5;

Nota: Se realiza el cambio, para que la cantidad de intento sea de 10.

const ATTEMPS = 10;


3) Tercer error, se esta haciendo una comparacion de igualdad estricta y esta estaba comparando
    con el número aleatorio, entonces se cambia el tipo de comparación y se indica que si la cantidad de veces fallida es mayor a 10 el usuario pierde. Que sería lo indicado en el inciso.

Error: if(userGuess === randomNumber)

Nota: Se realizan los cambios respectivos quedaría de la siguiente manera.

if(guessCount > ATTEMPS)

4) Cuarto error, se estaba haciendo nuevamente una comparación de igualdad estricta y estabán
    comparando con la cantidad de intento no con el número aleatorio como tal. Se realiza el cambio de comparación y se coloca la comparación con la variable que guarda el núemero aleatorio.

Error: else if(guessCount === ATTEMPS)

Nota: Se realizan las respectivos cambios.

else if(userGuess == randomNumber)
