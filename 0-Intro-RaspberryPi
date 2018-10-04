# 0. Introdución
Me dispongo a crear esta serie de documentos como soporte a mi aprendizaje con Raspberry Pi y Arduino.
# Raspberry Pi 2 Model B
Para poder utilizar la **Raspberry Pi 2B** (de ahí en adelante *raspi*) necesitamos volcar una versión de **Linux** compatible en una MicroSD. A continuación detallaré los pasos a seguir.

## Pasos (Windows)
 1. **Descargar** una versión Linux compatible. En nuestro caso **Raspbian**:
	https://www.raspberrypi.org/downloads/raspbian/
	> Podremos elegir entre descargar una versión con **escritorio** o una versión **sin** él (sólo dispondremos de la terminal). Esto dependerá del uso que le vayamos a dar. En mi caso descargo la versión con **escritorio *(Desktop).***

 2. **Formateamos** la MicroSD. Recomiendo el uso de **SDFormatter**, ya que evita posteriores problemas en Windows.
	 https://www.sdcard.org/downloads/formatter_4/
 3. **Volcamos la imagen** de **Raspbian** con la ayuda de **Win32DiskManager**. 
	- Seleccionamos la imagen.
	- Elegimos la unidad de la MicroSD.
	- Pulsamos *Write*.

## Activar SSH (sin conectar nada a la *raspi*)
Las nuevas versiones de Raspbian tienen **deshabilitado por seguridad SSH**.
> Más info: https://www.raspberrypi.org/blog/a-security-update-for-raspbian-pixel/

Para ello necesitaremos crear un fichero llamado **ssh** (este puede contener información o simplemente estar vacío) en la **partición boot de la MicroSD** 

> [!] **No confundir con la carpeta boot**. Es una partición montada llamada boot. Debes crear el archivo en la raíz.
