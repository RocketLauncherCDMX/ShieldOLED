# ShieldOLED
Shield OLED consta de una pantalla de 128x64 monocromática, 1 Joystick de 5 posiciones digital y 4 botones, todo por I2C

<br>

<p align="center">
  <img src="https://github.com/user-attachments/assets/dcdf06f8-bd02-4f81-98c5-084477218ea8" alt="Shield OLED 128x64" width="600"/>
</p>

---

Este shield es compatible con Arduino **UNO** y **MEGA**, y en teoría, cualquier tarjeta de desarrollo con la misma disposición de pines y del puerto **I2C**. Su principal caracteristica es la pantalla monocromática **OLED de 128 x 64 pixeles** que trae incorporada. Esta pantalla es ampliamente utilizada y funciona con el controlador **SSD1306**, cuyo manejo se puede hacer con algunas bibliotecas I2C diferentes.

<p align="center">
  <img src="https://github.com/user-attachments/assets/cebdb68c-9965-4e3e-93d1-0c78c1f04b5a" alt="Shield OLED 128x64" width="400"/>
</p>

El Joystickk es digital, de 5 posiciones, ideal para desplazarse por menús, seleccionar opciones, activar o desactivar actuadores, etc.
Los botones están en disposición de cruz, emulando un sencillo control de 8 bits.

Este shield es ideal para aprender conceptos básicos sobre gráficos, hacer interfaces sencillas para tus programas, modificar variables sin tener que compilar y programar cada vez, mostrar imágenes monocromáticas de baja resolución, y un largo etc.

Tanto la pantalla como el Joystick y los botones, funcionan por I2C, por lo que no será necesario que ocupes las entradas digitales o analógicas de tu Arduino.

---

## Primeros pasos

La pantalla se encuentra en la dirección **I2C 0x3C** y los botones y el Joystick en la dirección **I2C 0x02** por lo que se utilizan 2 librerias distintas. La biblioteca para la pantalla la puedes descargar de este link:

```bash 
https://github.com/adafruit/Adafruit_SSD1306.git
```
Y si tienes planeado utilizar formas geométricas como líneas, círculos y rectángulos, también deberás instalar esta otra:

```bash 
https://github.com/adafruit/Adafruit-GFX-Library
```
