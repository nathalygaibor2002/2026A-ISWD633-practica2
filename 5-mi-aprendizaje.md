# COMPLETAR  
En esta práctica aprendí a trabajar con redes y variables de entorno en Docker.
Pude entender cómo crear una red y cómo agregar contenedores dentro de la misma para que se comuniquen entre sí, como en el caso de WordPress y MySQL.
También aprendí a asignar variables de entorno para configurar datos importantes como usuarios, contraseñas y la conexión entre ambos servicios.
Lo que más me llamó la atención fue que al eliminar y volver a crear el contenedor de WordPress, la publicación y la configuración seguían apareciendo, porque la información se guardó en la base de datos MySQL.

Consultar: Cómo se gestionan datos confidenciales con los secretos de Docker (Docker Secrets).

Docker Secrets permite gestionar datos confidenciales como contraseñas, claves API y certificados de forma segura. Estos datos se almacenan cifrados dentro de Docker y se montan como archivos temporales dentro del contenedor en la ruta /run/secrets, evitando que la información sensible quede expuesta en el código o en variables de entorno visibles.
