# COMO USAR PANDOC
Instalar en el sistema paquetes necesarios.
```
sudo apt install texlive-latex-base texlive-latex-recommended texlive-latex-extra texlive-fonts-recommended texlive-fonts-extra
```
En la carpeta donde tengamos el archivo que queremos convertir crear una carpeta llamada `templates`

Dentro de esa carpeta meter los archivos necesarios para la comversion
- `eisvogel.tex`: para PDF.
- `github.html5`: para HTML.


Si el archivo para convertir es MARKDOWN para que quede mejor antes de todo se le podria poner una cabecera como esta.
```
---
title: "Titulo del arcivo"
author: [Nombre(Dejar los corchetes)]
subject: "Markdown"
keywords: [Markdown, README]
lang: "en"
toc-own-page: "true"
---
```
Ahora para convertir, abrir el script `test.bash.sh` y reemplazar las variables del principio
- `INPUT`: El archivo que quieres convertir.
- `OUTPUT_PDF`: Nombre del archivo cuando se convierta en PDF.
- `OUTPUT_HTML`: Nombre del archivo cuando se convierta en HTML.
- `OUTPUT_SLIDES`: Nombre del archivo cuando se convierta en SLIDES.

De esta forma simplemente ejecutar el script y haran las tres conversiones.