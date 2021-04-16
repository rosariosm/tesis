# Tesis ![Licencia](https://i.creativecommons.org/l/by-sa/4.0/88x31.png)

Este proyecto está basado en los fuentes de la [tesina](https://github.com/ncuesta/tesis)
 de grado de Miguel Carbone y
José Nahuel Cuesta Luengo, alumnos de la Facultad de Informática de la
Universidad Nacional de La Plata. Corresponde a la tesina de grado de Rosario Santa Marina, alumna de la UNLP, titulada *Adaptación de CodeCombat para la enseñanza de Python en la escuela secundaria*.

Este proyecto puede utilizarse como base para otros tesinistas que estén
interesados en realizar su informe documental con LaTeX, intentando facilitar el
proceso de aprendizaje inicial y el de organización del proyecto.

## Licencia

Este proyecto se encuentra licenciado bajo una [Licencia Creative Commons
Atribución-CompartirIgual 4.0 Internacional](http://creativecommons.org/licenses/by-sa/4.0/).

## Generación del PDF de salida

Al generar la salida, el resultado queda en el directorio `pdf/`.

### Con Docker

Primero, descargar la imagen del container para ejecutar Latex:

```console
$ docker pull ncuesta/latex
```

> La descarga de la imagen se hace sólo la primera vez.

Luego, cada vez que querramos ejecutar Latex para generar la salida en PDF:

```console
$ docker run --rm -v "`pwd`:/latex" -i ncuesta/latex
```

### Con PdfLaTeX instalado localmente

Se puede usar el `Makefile` de este directorio:

```console
$ make
```

# Buenas prácticas de Git

- Mensajes de commit: `#idClickup mensaje`. De esta manera se asocia nuestro commit a la tarjeta de clickup. Por ejemplo: `#3h9d71 Added something`.

- Nombre de PR: `#idClickup/Task name`. De esta manera se asocia nuestro PR a la tarjeta de clickup. Por ejemplo `#434zfz/Generate repo`


