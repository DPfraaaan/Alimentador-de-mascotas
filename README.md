# Alimentador-de-mascotas

El proyecto consiste en un alimentador automático de mascotas que consta de un tanque de comida y un plato que incluye una balanza para medir el peso de la comida que hay en él. Este dispositivo rellenará automáticamente el plato cuando esté vacío.

### Foto boceto:

https://medium.com/@lizeth.veraro/readme-qu%C3%A9-es-simples-pasos-para-crear-uno-4b82891626d7

### Funcionamiento: 
La cantidad de comida servida se podrá seleccionar mediante un botón que permitirá elegir entre perro grande, mediano y pequeño, con distintas configuraciones de llenado basadas en el peso. Además, otro botón permitirá cambiar la frecuencia con la que se rellena el plato, con intervalos de 4 horas.
El alimentador contará con una pantalla que mostrará información como la cantidad de comida en gramos en el plato y el tiempo restante para el próximo rellenado, en caso de que el animal haya consumido toda la comida del plato actual. Por último, incluirá un sensor ultrasónico que medirá el nivel del tanque. Si está lleno, se encenderá un LED verde; si está medio, un LED amarillo; y si está bajo, un LED rojo. Cuando el nivel esté muy bajo, se activará un buzzer como alarma.

### Componentes:
* Sensor ultrasonido (Hc-sr04)
* Leds (Verde ;Amarillo ;Rojo)
* Buzzer )
* Servo (sg-90)
* ESP-32
* Celda de carga (1kg) Hx711
* Pantalla LCD 16x2 I2C
* 2 Botones genéricos

### Comunicación entre módulos y MCU
* i2c ( pantalla LCD, Servo, sensor de ultrasonido ) 
* 2 pines (Clock y Data), de forma serial muy similar a I2C (celda de carga)
* PWM (servomotor ( como tal no es un sistema ) )

## Diagrama de conexión

![image](https://github.com/user-attachments/assets/da3c9469-515d-4984-9959-3e53d2369183)


## Boceto de diseño
![image](https://github.com/user-attachments/assets/394c5591-4e80-48ad-8e4a-1ace56f7a526)





