#react_intro
### Investigacion React.js

### ¿Que es React.js?
React.js es una biblioteca de JavaScript de código abierto utilizada para construir interfaces de usuario interactivas y dinámicas. Fue desarrollada por Facebook y se centra en la creación de componentes reutilizables que representan diferentes partes de la interfaz de usuario.
### ¿Cuáles son las diferencias entre React.js versión 18?
-Routing
-Rendering
-Data Fetching
-Styling
-Optimizations
-Typescript
Routing (Enrutamiento): React no tiene enrutamiento integrado por defecto, pero se utilizan bibliotecas externas como React Router para manejar el enrutamiento en las aplicaciones. En una versión 18 hipotética, podrían introducirse mejoras en la forma en que React interactúa con estas bibliotecas o podría haber un enfoque más integrado para manejar el enrutamiento.

Rendering (Renderización): React siempre ha estado enfocado en la eficiencia de la renderización, pero en una versión 18 podrían introducirse mejoras significativas en el algoritmo de renderización para optimizar el rendimiento, especialmente en aplicaciones con una gran cantidad de componentes.

Data Fetching (Obtención de datos): React no proporciona herramientas específicas para la obtención de datos, pero la forma en que los componentes interactúan con los datos (a través de solicitudes HTTP, por ejemplo) podría mejorar en términos de eficiencia y facilidad de uso en la versión 18.

Styling (Estilización): Aunque React no se enfoca directamente en la estilización, es común utilizar bibliotecas como styled-components o CSS modules para manejar estilos en aplicaciones React. En una versión 18, podrían introducirse mejoras en la forma en que se gestionan los estilos o en la integración de herramientas de estilización más avanzadas.

Optimizations (Optimizaciones): Cada nueva versión de React tiende a incluir mejoras en el rendimiento y la eficiencia. En una versión 18, podrían introducirse optimizaciones específicas para reducir el tiempo de carga, mejorar el rendimiento de la aplicación y hacer que React sea más eficiente en general.

Typescript: Aunque React es compatible con TypeScript, podría haber mejoras en la forma en que se integra con TypeScript en la versión 18. Esto podría incluir mejoras en la compatibilidad, la detección de errores y la facilidad de uso al trabajar con TypeScript en proyectos de React.
### Define los siguientes conceptos detrás de React:
components
JSX
props
state

Componentes: Son bloques de construcción reutilizables para interfaces de usuario. Los componentes pueden ser simples (como un botón) o complejos (como un formulario completo).

JSX: Es una extensión de JavaScript que permite escribir código que se parece a HTML dentro de JavaScript. JSX hace que sea más fácil y más intuitivo crear estructuras de componentes en React.

Props (Propiedades): Son datos que se pasan de un componente principal a un componente secundario. Los props permiten que los componentes sean configurables y reutilizables.

Estado (State): Es un objeto que representa la información relevante para un componente y puede cambiar durante la vida útil del componente. Cuando el estado de un componente cambia, React vuelve a representar el componente para reflejar ese cambio.
### Investiga sobre el patrón de diseño estructural llamado Composite, en qué consiste y cuál es su relación con React?
El patrón de diseño estructural llamado Composite se basa en la idea de componer objetos en una estructura de árbol para representar jerarquías de partes todo. En React, esto se relaciona con la composición de componentes para construir interfaces de usuario. Los componentes más pequeños se combinan para formar componentes más grandes, lo que facilita la creación y el mantenimiento de interfaces de usuario complejas.
### Investiga sobre el patrón de diseño estructural llamado State, en qué consiste y cuál es su relación con React?
El patrón de diseño estructural llamado State se centra en la gestión del estado de un objeto. En React, el estado de un componente es crucial para mantener y actualizar la información relevante para ese componente. React maneja el estado de manera eficiente, permitiendo que los componentes respondan a eventos y cambios de datos de manera dinámica. Esto facilita la creación de aplicaciones interactivas y receptivas.

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
