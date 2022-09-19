# Airlines

La tarea es predecir si un vuelo determinado se retrasará, dada la información de la salida programada.

![Flight_Delay-200x100](https://user-images.githubusercontent.com/111400931/191128895-632dd179-f4cb-4578-8723-04d0fb5577f8.png)

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

El equipo esta integrado por:
- Nicolas Duran
- Beltran Lacroze
- Javier Oro
- Lucas Misrahi

