#react_intro

### Tutorial Tic Tac Toe
### ¿Como Funciona el Juego:
El juego inicia con un tablero vacío y dos jugadores que toman turnos para marcar los cuadrados, uno con "X" y el otro con "O".
Cuando un jugador hace clic en un cuadrado vacio, el juego marca el cuadrado con el simbolo del jugador actual y verifica si hay un ganador.
Si hay un ganador o todos los cuadrados estan marcados, el juego termina. De lo contrario, el turno pasa al otro jugador.
El componente Game tambien permite a los jugadores revisar el historial de movimientos y volver a cualquier estado anterior del juego.
Este juego demuestra conceptos importantes de React como componentes, props, estado, y manejo de eventos.

### Resumen del juego:
El componente Square representa cada uno de los cuadrados del tablero. Recibe dos props: value (que puede ser "X", "O" o null, dependiendo de si el cuadrado está marcado o no) y onSquareClick, una función que se llama cuando se hace clic en el cuadrado.
Luego estan los componentes Board que representa el tablero del juego. Recibe las props xIsNext (un booleano que indica si el siguiente turno es de 'X'), squares (un arreglo que representa el estado actual del tablero) y onPlay, una función para manejar el movimiento en el tablero. Dentro de Board, se maneja el clic en los cuadrados y se determina si hay un ganador. 
Game es el componente principal que maneja el estado del juego, incluyendo el historial de movimientos (history), el movimiento actual (currentMove) y quién tiene el siguiente turno (xIsNext). Permite a los jugadores volver a cualquier estado anterior del juego a través de una lista de movimientos.
Y por ultimo esta la función calculateWinner, es una función auxiliar fuera de los componentes que toma el arreglo de squares como argumento y determina si hay un ganador, basándose en las posibles combinaciones ganadoras.
