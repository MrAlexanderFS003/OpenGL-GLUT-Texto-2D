# TEXTO EN PANTALLA 2D
Antes que todo este proyecto puede ser usado en proyectos que usen un plano en 3D .

Al momento de querer ejecutar el programa les saldra error, pero tranquilos, este error tiene una solución sencilla,
para solucionarlo tenemos que seguir lo siguiente:
> Copia lo siguiente: _CRT_SECURE_NO_WARNINGS

![Solucion](https://user-images.githubusercontent.com/96871746/212933383-9f5548fb-c07f-4a61-9e86-019d7020e7e3.gif)

> Programa en Ejecución:

![Ejm](https://user-images.githubusercontent.com/96871746/212933898-2f15a9ae-6764-4cbd-b84a-bfa5aac29532.gif)

### Modificar fuente de letras
El siguiente código solo es para ejemplo , no esta completo.
Para modificar la fuente de letra nos guiaremos de esta pag.

> https://www.opengl.org/resources/libraries/glut/spec3/node76.html#SECTION000111000000000000000

Cada *font_style* guarda el tipo de fuente de la letra , quizas no hay muchas fuentes , pero hay librerias que ayudan con mas variedad.
```C++
void Texto::printw(int val, float x, float y, float z, const char* format, ...) {
	if (val == 1) {
		font_style = GLUT_BITMAP_TIMES_ROMAN_10; 
	}
	else {
		font_style = GLUT_BITMAP_TIMES_ROMAN_24;
	}
}
```
