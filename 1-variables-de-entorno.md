# Variables de Entorno
### ¿Qué son las variables de entorno?

Las variables de entorno en Docker son valores que se le pasan a un contenedor para configurar su comportamiento sin modificar el código de la aplicación.

### Para crear un contenedor con variables de entorno

```
docker run -d --name <nombre contenedor> -e <nombre variable1>=<valor1> -e <nombre variable2>=<valor2>
```

### Crear un contenedor a partir de la imagen de nginx:alpine con las siguientes variables de entorno: username y role. Para la variable de entorno rol asignar el valor admin.


<img width="1193" height="70" alt="image" src="https://github.com/user-attachments/assets/98ddd268-fc9c-4605-95a3-1684d51c9e8f" />


# CAPTURA CON LA COMPROBACIÓN DE LA CREACIÓN DE LAS VARIABLES DE ENTORNO DEL CONTENEDOR ANTERIOR

<img width="1236" height="974" alt="image" src="https://github.com/user-attachments/assets/3e1c73f9-4c68-4ad7-b021-4f5d405d00f8" />


### Crear un contenedor con la imagen de mysql, mapear todos los puertos

<img width="842" height="68" alt="image" src="https://github.com/user-attachments/assets/3d55eea8-53f8-4ff4-8432-37a4d5ef15ac" />


### ¿El contenedor se está ejecutando?
No
### Identificar el problema
No estan configuradas las variables de entorno, el root.
### Para crear un contenedor con variables de entorno especificadas
- Portabilidad: Las aplicaciones se vuelven más portátiles y pueden ser desplegadas en diferentes entornos (desarrollo, pruebas, producción) simplemente cambiando el archivo de variables de entorno.
- Centralización: Todas las configuraciones importantes se centralizan en un solo lugar, lo que facilita la gestión y auditoría de las configuraciones.
- Consistencia: Asegura que todos los miembros del equipo de desarrollo o los entornos de despliegue utilicen las mismas configuraciones.
- Evitar Exposición en el Código: Mantener variables sensibles como contraseñas, claves API, y tokens fuera del código fuente reduce el riesgo de exposición accidental a través del control de versiones.
- Control de Acceso: Los archivos de variables de entorno pueden ser gestionados con permisos específicos, limitando quién puede ver o modificar la configuración sensible.

### ¿Qué bases de datos existen en el contenedor creado?

<img width="1072" height="381" alt="image" src="https://github.com/user-attachments/assets/3d46cdda-32fa-40e6-ab8e-cf9c0f8875bb" />

