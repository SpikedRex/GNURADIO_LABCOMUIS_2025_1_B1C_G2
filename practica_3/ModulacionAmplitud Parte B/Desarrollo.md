| Simulación GNU Radio | Osciloscopio | Analizador De Espectros | Tiempo de Bit | Índice De Modulación | Ancho de Banda de la Señal |
|-----------------|-----------------------| -----------------------| -----------------------|-----------------------|-----------------------|
| <img src="punto_1/Caso1SimulacionGNURadio.PNG"> | <img src="punto_1/Caso1Osciloscopio.PNG"> | <img src="punto_1/Caso1AnalizadorDeEspectros.PNG"> | 2 ns | 0.714 |  313.028 kHz |
| <img src="punto_1/Caso2SimulacionGNURadio.PNG"> | <img src="punto_1/Caso2Osciloscopio.PNG"> | <img src="punto_1/Caso2AnalizadorDeEspectros.PNG"> | 3.2 µs | 0.999 | 9.406 MHz |
| <img src="punto_1/Caso3SimulacionGNURadio.PNG"> | <img src="punto_1/Caso3Osciloscopio.PNG"> | <img src="punto_1/Caso3AnalizadorDeEspectros.PNG"> | 3.2 µs | 115.126 |   |

Se puede observar en los resultados obtenidos que, para cada caso, el índice de modulación es ligeramente menor al valor asignado. Esta disminución se debe muy probablemente a pérdidas durante la transmisión de la señal. Además, el espectro de la señal mostrado en el analizador de espectros presenta un ancho de banda similar al esperado según la simulación.

En el primer caso, correspondiente a una modulación de 4 bits con un indice de 75 %, es posible observar claramente los cuatro niveles (escalones) simulados en el osciloscopio. Sin embargo, al aumentar el índice de modulación por encima del 100 %, como en el caso 3 (120 %), se observa en el osciloscopio que solo se distinguen tres niveles. Esto indica que, al superar un índice de modulación del 100 %, comienza a perderse información en la señal modulada. En nuestro caso particular, se perdió un bit de información.


| Simulación GNU Radio | Osciloscopio | Analizador De Espectros| Índice De Modulación | Ancho de Banda de la Señal |
|-----------------|-----------------------| -----------------------| -----------------------|-----------------------|
| <img src="punto_2/Caso1SimulacionGNURadio.PNG"> | <img src="punto_2/Caso1Osciloscopio.PNG"> | <img src="punto_2/Caso1AnalizadorDeEspectros.PNG"> | 0.561 | 74.45 kHz |
| <img src="punto_2/Caso2SimulacionGNURadio.PNG"> | <img src="punto_2/Caso2Osciloscopio.PNG"> | <img src="punto_2/Caso2AnalizadorDeEspectros.PNG"> | 0.8685 | 70.22 kHz |
| <img src="punto_2/Caso3SimulacionGNURadio.PNG"> | <img src="punto_2/Caso3Osciloscopio.PNG"> | <img src="punto_2/Caso3AnalizadorDeEspectros.PNG"> | 1.1838 | 78.68 kHz |

Se puede observar que en todos los casos analizados, el índice de modulación medido fue ligeramente inferior al valor configurado en la simulación. Específicamente, se detectó una reducción que varió entre un 1 % y un 14 %. Si bien esta reducción era de esperarse debido a posibles limitaciones físicas, pérdidas duránte la transmisión o problemas de ganancia en el USRP, no afectó significativamente la visualización del comportamiento de la señal modulada. En todos los casos, la forma de onda observada coincidió con lo esperado para el índice de modulación asignado.

Por otro lado, al analizar las señales en el analizador de espectros, se comprobó que el ancho de banda estimado para cada caso fue muy cercano al valor simulado en GNU radio. Además, el comportamiento espectral fue similar. Finalmente, se observó que el piso de ruido del sistema no llegó a afectar la señal modulada, ya que esta se mantuvo claramente por encima del nivel de ruido. Esto indica que la señal puede ser recibida de manera adecuada sin sufrir pérdidas significativas por interferencia del piso de ruido.

