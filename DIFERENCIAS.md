# Diferencias entre Bootstrap y Materialize

Ambas versiones (`/` con Bootstrap y `/materialize` con Materialize) hacen lo mismo: menú,
extracto centrado, productos y formulario de contacto, con la misma paleta de rojos.

- **Grilla**: en Bootstrap se usa `col-12 col-md-4`, en Materialize `col s12 m4`. Ambas dividen
  la pantalla en 12 columnas, pero Materialize junta el tamaño de pantalla y el número de
  columnas en una sola letra (s = celular, m = tablet, l = escritorio).

- **Menú**: en Bootstrap se usa la clase `navbar`, en Materialize `nav` + `nav-wrapper`. Se ven
  parecidos, pero en esta versión simplificada no se agregó el menú hamburguesa para celulares,
  así que en pantallas chicas los links del menú se ven más apretados en Materialize.

- **Formulario**: Bootstrap usa `form-control` y se ve bien sin necesitar JavaScript. Materialize
  necesita normalmente JavaScript (`M.updateTextFields()`) para que las etiquetas "floten" sobre
  el input; en esta versión simple se evitó ese JS y se dejaron las etiquetas fijas arriba con la
  clase `active`.

- **Imágenes responsivas**: Bootstrap usa `img-fluid`, Materialize usa `responsive-img`. Cumplen
  la misma función.

- **Colores**: los dos frameworks traen sus propios colores por defecto (azul en Bootstrap, verde
  en Materialize), por lo que en ambos casos se sobrescribió con CSS propio (`assets/style.css`)
  para dejar todo en tonos rojos.
