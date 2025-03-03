# Práctica 1A: GNU Radio para el procesamiento de señales

### Integrantes
- **DANILO ALEXANDER DURÁN MEJÍA** - 2210405
  
Escuela de Ingenierías Eléctrica, Electrónica y de Telecomunicaciones  
Universidad Industrial de Santander

### Fecha
03 de Marzo de 2025

---

## Punto 1
  Arcivo .grc: [`Lab_comu_1.grc`](https://github.com/SpikedRex/GNURADIO_LABCOMUIS_2025_1_B1C_G2/blob/main/practica_1/practica_1A/Lab_comu_1.grc)   
  Arcivo .py: [`Lab_comu_1.py`](https://github.com/SpikedRex/GNURADIO_LABCOMUIS_2025_1_B1C_G2/blob/main/practica_1/practica_1A/Lab_comu_1.py)

## Punto 2
  Señal seno operando a una frecuencia de 100 Hertz

  [`Lab_comu_1_2.grc`](https://github.com/SpikedRex/GNURADIO_LABCOMUIS_2025_1_B1C_G2/blob/main/practica_1/practica_1A/Lab_comu_1_2.grc)
  
  <img src="https://github.com/SpikedRex/GNURADIO_LABCOMUIS_2025_1_B1C_G2/blob/main/practica_1/practica_1A/Punto%202%20-%20Seno%20100%20Hz.png" alt="Punto 2" width="1200">

## Punto 4
  Señal TRIANGULAR tipo flotante operando a una frecuencia de 4500 Hertz y amplitud 3

  [`Lab_comu_1_4.grc`](https://github.com/SpikedRex/GNURADIO_LABCOMUIS_2025_1_B1C_G2/blob/main/practica_1/practica_1A/Lab_comu_1_3.grc)
  
  <img src="https://github.com/SpikedRex/GNURADIO_LABCOMUIS_2025_1_B1C_G2/blob/main/practica_1/practica_1A/Punto%204%20-%20Triangular%204500%20Hz%203%20Amp.png" alt="Punto 4" width="1200">

## Punto 5
#### 1. Demostrar los efectos sobre la forma de onda cuando se tiene una relación de muestreo (samp_rate/Frequency = 5). Describa en un párrafo las desventajas o ventajas al llegar a este límite; apoye su argumento con una imagen.
  La gráfcia obtenida es de una función sierra una frecuencia de 2 K Hz y una frecuencia de muestreo de 10 K Hz, es posible apreciar que con esta relación de muestreo, se logra capturar una buena forma de la señal original, sin embargo, tomar mayor cantidad de muestras representa un costo computacional mayor ya que son mas datos los que se guardan y se necesitan procesar.

  [`Lab_comu_1_5.grc`](https://github.com/SpikedRex/GNURADIO_LABCOMUIS_2025_1_B1C_G2/blob/main/practica_1/practica_1A/Lab_comu_1_4.grc)
  
  <img src="https://github.com/SpikedRex/GNURADIO_LABCOMUIS_2025_1_B1C_G2/blob/main/practica_1/practica_1A/Punto%205%20-Relacion5.png" alt="Punto 5" width="1200">

#### 2. Asignando bloque QT GUI Range para la variable samp_rate. Inserte una grafica donde demuestre la ventaja comparativa de trabajar con la relacion de muestreo = 5 frente al limite de Nyquist. Demestre usando al menos una forma de onda diferente a la señal senoidal.
 
  <img src="https://github.com/SpikedRex/GNURADIO_LABCOMUIS_2025_1_B1C_G2/blob/main/practica_1/practica_1A/Punto%205%20-NysquitYRelacion.png" alt="Punto 5" width="1200">
  <img src="https://github.com/SpikedRex/GNURADIO_LABCOMUIS_2025_1_B1C_G2/blob/main/practica_1/practica_1A/Punto%205%20-%20NysquitYRelacion_2.png" alt="Punto 5" width="1200">

## Punto 6
  La gráfica obtenida corresponde a un Seno de frecuencia 2 K Hz y una frecuencia de muestreo de 40 K Hz, por lo tanto, se tiene una relación samp_rate/frequency de 20. Es posible apreciar que para esta relación, se recupera muy bien la señal original.
  <img src="https://github.com/SpikedRex/GNURADIO_LABCOMUIS_2025_1_B1C_G2/blob/main/practica_1/practica_1A/Punto%206.PNG" alt="Punto 6" width="1200">

  
