## **Mini-Proyecto del [tema 2](../tema2.md)**

### Skylab Airlines! ✈️🛩

_(Los datos de los vuelos están al final del enunciado, podéis usarlos en vuestro código)_

Programa una inferfaz de usuario para una aerolinea (por terminal...). Esta aerolinea dispondrá de 10 vuelos para el dia de hoy, para empezar, estos vuelos estarán declarados de manera global, cuando se llame a la función:

-   Se preguntará por el nombre de usuario y dará la bienvenida.
-   El usuario visualizará todos los vuelos disponibles de una forma amigable:
    El vuelo con origen: _Barcelona_, y destino: _Madrid_ tiene un coste de _XXXX€_ y no realiza _ninguna_ escala.
-   A continuación, el usuario verá el coste medio de los vuelos.
-   También podrá ver cuantos vuelos efectúan escalas.
-   Sabiendo que los ultimos 5 vuelos (los últimos 5 ID's) son los últimos del día, muestra al usuario sus destinos.

**PRO!:**

Después de ver toda la información el programa pedirá al usuario si es ADMIN/USER, dependiendo de la elección, el programa se comportará de la siguiente manera:

Si eres _ADMIN_, la función debería permitir:

-   Poder crear, más vuelos, pidiendo la información por prompt(), sin poder pasar de 15 vuelos, si se intenta introducir uno más, saltará un alert().
-   Poder eliminar vuelos mediante el ID.

Si eres _USER_ la función debería permitir:

-   Buscar por precio (más alto, más bajo o igual), el usuario debería mostrar los datos de los vuelos encontrados y, indicando el ID, el programa responderá:
    "Gracias por su compra, vuelva pronto."

```js
var flights = [
    { id: 00, to: 'Bilbao', from: 'Barcelona', cost: 1600, scale: false },
    { id: 01, to: 'New York', from: 'Barcelona', cost: 700, scale: false },
    { id: 02, to: 'Los Angeles', from: 'Madrid', cost: 1100, scale: true },
    { id: 03, to: 'Paris', from: 'Barcelona', cost: 210, scale: false },
    { id: 04, to: 'Roma', from: 'Barcelona', cost: 150, scale: false },
    { id: 05, to: 'London', from: 'Madrid', cost: 200, scale: false },
    { id: 06, to: 'Madrid', from: 'Barcelona', cost: 90, scale: false },
    { id: 07, to: 'Tokyo', from: 'Madrid', cost: 1500, scale: true },
    { id: 08, to: 'Shangai', from: 'Barcelona', cost: 800, scale: true },
    { id: 09, to: 'Sydney', from: 'Barcelona', cost: 150, scale: true },
    { id: 10, to: 'Tel-Aviv', from: 'Madrid', cost: 150, scale: false }
];

console.log(flights[0].to); //output: Bilbao
```
