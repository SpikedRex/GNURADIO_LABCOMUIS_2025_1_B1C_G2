# Práctica 1B: Reconociendo equipos

### Integrantes
- **DANILO ALEXANDER DURÁN MEJÍA** - 2210405
  
Escuela de Ingenierías Eléctrica, Electrónica y de Telecomunicaciones  
Universidad Industrial de Santander

### Fecha
03 de Marzo de 2025

---

## Punto 1
#### 1. ¿De que depende la precisión de medida en el osciloscopio? (describa en no menos de 50 palabras)

  La precisión de medida en el osciloscopio depende de varios factores. Uno de ellos es el cable de comunicación entre el USRP-2920 y el osciloscopio, ya que puede generar pérdidas en la señal o provocar ruido, esto depende de la calidad y longitud. Además, tanto el osciloscopio como el USRP-2920, pueden agregar ruido que afecta la medición. Por otro lado, si la señal que se mide supera los rangos mínimo o máximo del osciloscopio, la medición puede verse afectada por saturación o falta de resolución, lo que impide obtener resultados precisos.

#### 2. Determine el porcentaje de amplitud de la señal recibida con respecto a la señal generada desde el PC. Es igual para todos los casos, en caso de ser diferente ¿a que atribuye esta caída de tensión. (describa en no menos de 50 palabras)

#### Caso 1: gtx=10

Arcivo .xlsx: [`Práctica1B-Punto1.xlsx`](https://github.com/SpikedRex/GNURADIO_LABCOMUIS_2025_1_B1C_G2/blob/main/practica_1/practica_1B/Pr%C3%A1ctica1B-Punto1.xlsx)

| Amplitudes (mV) | Amplitud Generada (mV) | Vamp Medida PP (mV) | Amplitud Medida (mV) | Porcentaje |
|-----------------|-----------------------|----------------------|----------------------|------------|
| 500            | 87.94                 | 556.2               | 278.1               | 55.62 %    |
| 250            | 43.64                 | 276.0               | 138.0               | 55.20 %    |
| 125            | 22.13                 | 139.95              | 70.0                | 55.98 %    |
| 62.5           | 11.07                 | 70.0                | 35.0                | 56.00 %    |

<img src="https://github.com/SpikedRex/GNURADIO_LABCOMUIS_2025_1_B1C_G2/blob/main/practica_1/practica_1B/GraphCaso1.PNG" alt="Punto 2" width="1200">

#### Caso 2: gtx=20

| Amplitudes (mV) | Amplitud Generada (mV) | Vamp Medida PP (mV) | Amplitud Medida (mV) | Porcentaje |
|-----------------|-----------------------|----------------------|----------------------|------------|
| 500            | 153.09                 | 968.24              | 484.1               | 96.82 %    |
| 250            | 80.53                  | 509.33              | 254.7               | 101.87 %   |
| 125            | 40.39                  | 255.42              | 127.7               | 102.17 %   |
| 62.5           | 20.37                  | 128.8               | 64.4                | 103.04 %   |

<img src="https://github.com/SpikedRex/GNURADIO_LABCOMUIS_2025_1_B1C_G2/blob/main/practica_1/practica_1B/GraphCaso2.PNG" alt="Punto 2" width="1200">

#### Caso 3: gtx=30

| Amplitudes (mV) | Amplitud Generada (mV) | Vamp Medida PP (mV) | Amplitud Medida (mV) | Porcentaje |
|-----------------|-----------------------|----------------------|----------------------|------------|
| 500            | 316.23                 | 2000.00             | 1000.0              | 200.00 %   |
| 250            | 134.50                 | 850.64              | 425.3               | 170.13 %   |
| 125            | 72.05                  | 455.7               | 227.9               | 182.28 %   |
| 62.5           | 37.99                  | 240.24              | 120.1               | 192.19 %   |

<img src="https://github.com/SpikedRex/GNURADIO_LABCOMUIS_2025_1_B1C_G2/blob/main/practica_1/practica_1B/GraphCaso3.PNG" alt="Punto 2" width="1200">

Es posible apreciar de las anteriores gráficas que a medida que aumenta la ganancia de transmisión (GTX), el porcentaje de amplitud de la señal medida con respecto a la señal generada también aumenta. En otras palabras, a mayor gtx, mayor perdida de la amplitud. Cada 10 puntos que aumete gtx, la perdida aumenta el doble. Este comportamiento es debido a diversos fáctores tales como el cable de conexión y su longitud ademas de que aumentar el gtx tambíen puede aumentar el ruido del sistema, haciendo que la presicion del osciloscopio se vea afectada.

#### Fotos de las señales medidas:
| ![Imagen 1](WhatsApp%20Image%202025-03-03%20at%208.36.37%20PM%20(1).jpeg) | ![Imagen 2](WhatsApp%20Image%202025-03-03%20at%208.36.37%20PM%20(2).jpeg) | ![Imagen 3](WhatsApp%20Image%202025-03-03%20at%208.36.37%20PM.jpeg) |
|---|---|---|
| ![Imagen 4](WhatsApp%20Image%202025-03-03%20at%208.36.38%20PM%20(1).jpeg) | ![Imagen 5](WhatsApp%20Image%202025-03-03%20at%208.36.38%20PM%20(2).jpeg) | ![Imagen 6](WhatsApp%20Image%202025-03-03%20at%208.36.38%20PM.jpeg) |
| ![Imagen 7](WhatsApp%20Image%202025-03-03%20at%208.36.39%20PM%20(1).jpeg) | ![Imagen 8](WhatsApp%20Image%202025-03-03%20at%208.36.39%20PM%20(2).jpeg) | ![Imagen 9](WhatsApp%20Image%202025-03-03%20at%208.36.39%20PM%20(3).jpeg) |
| ![Imagen 10](WhatsApp%20Image%202025-03-03%20at%208.36.40%20PM%20(1).jpeg) | ![Imagen 11](WhatsApp%20Image%202025-03-03%20at%208.36.40%20PM%20(2).jpeg) | ![Imagen 12](WhatsApp%20Image%202025-03-03%20at%208.36.40%20PM.jpeg) |
