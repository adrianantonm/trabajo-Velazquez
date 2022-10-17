# DOCUMENTACIÓN
## INTRODUCCIÓN
Esta práctica se trata de crear una página web con un repositorio en git utilizando html, css y JavaScript.
Debería ser lo más responsive posible para que se pueda ajustar a cualquier dispositivo.
* Lenguajes:
  * HTML
  * CSS
  * JAVASCRIPT


## PARTES DE TRABAJO
### COMMIT 1 (maquetación)

He creado los directorios y archivos html (contenido de la página), css (personalización), js (interactividad de la
página), readme (para documentar el proyecto), .gitignore (ignora los archivos o directorios que quiera como las
imágenes y .idea) y un repositorio con el comando git init, con git add . se preparan los archivos y directorios .

Se ha estructurado el contenido en un header para el titulo, y tres section, para la barra de imágenes pequeñas, la 
imagen grande y la descripción. En el css se ha ajustado el tamaño de los section y se ha introducido la letra a 
utilizar.

Por último se ha hecho un commit.

### COMMIT 2 (barra lateral)

Se han introducido las imágenes pequeñas de la izquierda, ajustadas de tamaño, centradas con css, con un filtro blanco 
y negro que cuando pasas el mouse se vuelve con el color original (hover) con una transición de 1s (transition) y con 
una barra de desplazamiento en el section (overflow-y:scroll).

### COMMIT 3 (imágenes y descripción)

Se han introducido las imágenes grandes dentro de un section y en un div cada una, lo mismo se ha hecho con la 
descripción de la derecha. En el css se ha ajustado la altura de la descripción, el grosor de la letra, el texto se ha 
centrado y por último se ha modificado el button quitando el borde (border:none), y cuando pases el mouse cambie de 
color de fondo (hover)

### COMMIT 4 (cambio de cuadro y responsive)
Se han creado las páginas para enlazar más adelante en la imágenes grandes del medio y un solo archivo css para ajustar 
todas las imágenes en una vez y se ha enlazado el archivo JavaScript después del body.

* Código JavaScript

```JavaScript
    let tabs = document.querySelectorAll('.pequeño'),
    contents = document.querySelectorAll('.contenido');

    tabs.forEach((tab, index) => {
    tab.addEventListener('click', () => {
    contents.forEach((content) => {
    content.classList.remove('is-active');
    });
    tabs.forEach((tab) => {
    tab.classList.remove('is-active');
    });

    contents[index].classList.add('is-active');
    tabs[index].classList.add('is-active');
    });
    });
```
Con este código conseguimos que al hacer click encima de una imagen cambie el section en el que esta la imagen grande, 
con la descripción lo logro más adelante cambiando las secciones de la descripcion dentro de la sección de las 
imágenes grandes.

### COMMIT 5 (imágenes grandes)

Se ha creado un enlace en las imágenes grandes hacia las páginas de las imágenes, he introducido cada imagen su página 
correspondiente y en el css se centró la imagen en el medio y con un fondo negro.

### COMMIT 6 (retoques)

En esta parte no he cambiado muchas cosas solo he modificado el css de las imágenes grandes porque no habia quedado
del todo centrado y algo del css de la página principal como el color de fondo del header para que no se superponga la 
imágen grande al hacer scroll.

### COMMIT 7 (final)
