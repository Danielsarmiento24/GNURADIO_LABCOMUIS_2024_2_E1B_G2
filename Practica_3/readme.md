El objetivo de este laboratorio fue estudiar y analizar el comportamiento de la modulación de amplitud (AM) y las modulaciones lineales en un entorno controlado utilizando
herramientas analíticas como un osciloscopio, GNU Radio y un analizador de espectro. Creando y procesando una señal de mensaje, se evaluaron diferentes
configuraciones de índice de modulación, ganancia y frecuencia portadora para comprender mejor la influencia de estos parámetros en el espectro de la señal modulada.

Parte A: Modulaciones Lineales 
En esta parte, se utilizó GNU Radio para representar la señal modulada en banda base mediante su envolvente compleja. Este modelo en banda base facilita la
observación de las características de la señal en el dominio del tiempo y la frecuencia sin necesidad de trabajar directamente con la señal de alta frecuencia. Se probaron tres configuraciones de la envolvente
compleja para la modulación AM:
● Caso 1: ka×Am=1
● Caso 2: ka×Am>1
● Caso 3: ka×Am<1
Mediciones de Potencia: Para cada caso, se midió la potencia de la portadora, las bandas laterales superior e inferior, y el índice de modulación utilizando el analizador de espectro y el bloque de medición de
potencia en GNU Radio. Además, se registraron las diferencias de potencia observadas en cada banda.
Tambien se midio el   índice de modulación (ka*Am) se calcula por medio de:
NdB = 20 log10 (ka*Am/2)
![image](https://github.com/user-attachments/assets/9266b82d-6a09-423e-8fc5-658c23696909)

![image](https://github.com/user-attachments/assets/cae35bde-7ee2-44c6-afc5-940f34eebb57)

![evidencia como medir frecuencia osciloscopio](https://github.com/user-attachments/assets/5f97beda-b3a3-49a9-b187-afcc10d3345a)
En esta practica aprendi a identificar las señales sobremoduladas submoduladas y moduladas, tambien que el índice de modulación es un parámetro clave para determinar la calidad de la señal.
El laboratorio me  permitió comprender cómo varían las características de la señal modulada en función del índice de modulación y la frecuencia portadora en sistemas de modulación en amplitud.


Adjunto tablas de evidencia https://docs.google.com/spreadsheets/d/1oss404eMRR9C0D6AIvPfBZg7CLzfMg9uvShGy5-CnF8/edit?usp=sharing

Parte B: Modulación en Amplitud (AM)
Se configuró una fuente de datos binaria aleatoria en GNU Radio con media cero. Esta señal fue utilizada como señal de mensaje en la modulación de amplitud. Implementación de la Modulación AM: Se utilizaron
los bloques de modulación de amplitud de prácticas anteriores para modular la señal de mensaje con una señal portadora. Se generaron tres configuraciones de modulación con índices de modulación del 75%, 100%, y 150%.
● Caso 1: Modulación del 75% con frecuencia deportadora de 300 MHz, ganancia de transmisión de 10 dB y 10 muestras por símbolo.
● Caso 2: Modulación del 100% con frecuencia deportadora de 250 MHz, ganancia de transmisión de 15 dB y 5 muestras por símbolo.
● Caso 3: Modulación del 150% con frecuencia deportadora de 350 MHz, ganancia de transmisión de 20 dB y 2 muestras por símbolo.
Mediciones de la Señal: Para cada caso, se midió el índice de modulación y el tiempo de bit usando un osciloscopio. También se utilizó un analizador de espectropara medir el ancho de banda de la señal modulada, y se
observó el comportamiento de la señal en el dominio de la frecuencia.
Asu vez tambien se analizo como seria con una señal de audio y las siguientes indicaciones 
1. Genere una Señal modulada en 60 %; Frecuencia de portadora 300 MHz, Ganancia de TX = 10 dB,
2. Genere una Señal modulada en 100 %; Frecuencia de portadora 250 MHz, Ganancia de TX = 15 dB,
3. Genere una Señal modulada en 120 %; Frecuencia de portadora 350 MHz, Ganancia de TX = 20 dB,

![parte 3 b  señal 2 analizador](https://github.com/user-attachments/assets/f023af29-8a9c-4416-a34e-e7e7bd8471c6)

En esta parte del laboratorio aprendi que a medida que aumenta el índice de modulación, también aumenta el ancho de banda ocupado por la señal. En el caso de la sobremodulación, el ancho de banda es mayor,lo cual puede ser un problema en entornos donde el ancho de banda es limitado.Tambien que la  cantidad de muestras por símbolo afecta la precisión con la que la señal de mensaje es representada en la señal modulada. Una menor cantidad de muestras por símbolo reduce la resolución temporal y puede hacer que la señal aparezca escalonada o menos precisa

Adjunto enlace a excel con los datos https://docs.google.com/spreadsheets/d/1ITrQqKQa1S7jeqcPcN-EvbeikLnNdCixtEXV4y0h1yg/edit?usp=sharing
