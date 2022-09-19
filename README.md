# Airlines + Proyecto Final + Coder House

El equipo esta integrado por:
- Nicolas Duran
- Beltran Lacroze
- Javier Oro
- Lucas Misrahi

# Resumen

La tarea es predecir si un vuelo determinado se retrasará, dada la información de la salida programada.

![Flight_Delay-200x100](https://user-images.githubusercontent.com/111400931/191128895-632dd179-f4cb-4578-8723-04d0fb5577f8.png)

Las variables en su mayoria son categoricas, para considerarlas en nuestro estudio se realizara el metodo de "One-Hot Encoding" para cada una de las categorias de cada variable categorica, haciendo un top 20 como max, logrando asi considerar todas las variables. Esto metodo de top 20 se realizara para no generar un alto rendimiento de los procesadores y facilitar la realizacion del estudio computacional.

Se buscara a travez de este estudio:
+ Si los aeropuertos juegan un papel importante en las demoras.
+ Si dependera mas de la duracion y largo del vuelo.
+ Que papel juegan las aerolineas.
+ Si dependera del dia de la semana.

Permitira identificar al cliente por que aerolinea optar, y cuales son los aeropuertos de origen y destino de debera tener cuidado para programar mejor sus tiempos.

1. Airline (Nombre de la aerolinea)
2. Flight (Numero de vuelo)
3. Airport From (Aeropuerto Origen)
4. Airport To (Aeropuerto Destino)
5. DayOfWeek (Dia de la semana)
6. Time (Duracion del vuelo)
7. Length (Distancia recorrida)
8. Delay (Si llego tarde o no)

Las variables categoricas son:
- Airline
- Flight
- Airport From
- Airport To
- DayOfWeek
- Delay

Descripcion de variables:
- Airline: Se aplicara el metodo "One-Hot Encoding" para poder realizar las posteriores analisis.
- Fligth: En principio se tomara como variable debil dado que es el nombre del vuelo, no deberia afectar en la duracion.
- Airport From y Airport To : Primero se realizara un top20 y se agrupara el resto, para poder aplicar el metodo "One-Hot Encoding" para los posteriores analisis.
- DayOfWeek: Si bien es type Int64 sigue siendo variable categorica por lo que se aplicara el metodo "One-Hot Encoding".
- Delay: 1 Demorado - 0 a Tiempo. Es la variable dependiente de nuestro estudio.

Las variables numericas son:
- Time
- Length
