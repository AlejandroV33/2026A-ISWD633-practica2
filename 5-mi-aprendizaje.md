# Mi aprendizaje
### Variables de entorno
Ya tenía conocimiento de qué eran las variables de entorno, las había usado para configurar cosas como Java, Python, etc. En mi computadora en local. Pero es la primera vez que las uso en contenedores y entiendo su importancia con ciertas imagenes, especialmente bases de datos.

### Ejercicio (2)
Para la practica 2-ejercicio me encontre con el problema de que no menciona el paso de crear una red para que se puedan comunicar ambos contenedores, sin embargo luego de una pequeña busqueda y posterior lectura de la práctica 3-redes me quedo claro como crear una red y añadir los contenedores.

### Redes
Ya tenía todo el conocimiento básico de redes pero no las había usado antes en dcoker, con esta práctica me quedó claro los tipos de redes que existen en Docker (bridge, host, none) y cuando se usan.

### Ejercicio (2)
Aprendí cómo levantar y configurar un servidor de WordPress. Sin embargo tuve un funcionamiento inesperado al eliminar y volver a agregar el contendor con el servidor de WordPress ya que asumí que todo se guardaba en la base de datos que estaba en el otro contenedor, sin embargo al volover a iniciar el contendor solo obtenia una pantalla en blanco en el navegador y no pude solucionar esto para acceder al panel de administración de WordPress.

## Cómo se gestionan datos confidenciales con los secretos de Docker (Docker Secrets).
Los secretos de Docker se gestionan almacenando información sensible (como contraseñas, claves API o certificados) de forma cifrada en el clúster y nunca dentro de la imagen del contenedor ni en variables de entorno visibles; cuando un servicio los necesita, Docker los monta de manera temporal como archivos dentro del contenedor en rutas seguras (por defecto en /run/secrets/), con acceso restringido solo a los servicios autorizados, y además estos datos se transmiten de forma segura entre nodos y se eliminan automáticamente cuando el contenedor se detiene, lo que reduce el riesgo de exposición accidental o filtraciones.
