## Esquema para el ejercicio
![Imagen](esquema-4-ejercicio.PNG)

### Crear la red

<img width="682" height="65" alt="image" src="https://github.com/user-attachments/assets/35557208-5bb7-4259-8831-68617f89073f" />

### Crear el contenedor mysql a partir de la imagen mysql:8, configurar las variables de entorno necesarias

<img width="1448" height="347" alt="image" src="https://github.com/user-attachments/assets/04d9d2b1-bf58-4a5f-963a-a8904220af86" />

### Crear el contenedor wordpress a partir de la imagen: wordpress, configurar las variables de entorno necesarias

<img width="1462" height="584" alt="image" src="https://github.com/user-attachments/assets/ba6408d5-b046-40fd-ba4f-82d1e7b95596" />

De acuerdo con el trabajo realizado, en el esquema del ejercicio el puerto a es **(completar con el valor)**

Ingresar desde el navegador al wordpress y finalizar la configuración de instalación.

<img width="947" height="865" alt="image" src="https://github.com/user-attachments/assets/0fd64984-6980-4bfb-a84c-3b96adabf873" />

Desde el panel de admin: cambiar el tema y crear una nueva publicación.
Ingresar a: http://localhost:9300/ 
recordar que a es el puerto que usó para el mapeo con wordpress
# COLOCAR UNA CAPTURA DEL SITO EN DONDE SEA VISIBLE LA PUBLICACIÓN.

<img width="1882" height="826" alt="image" src="https://github.com/user-attachments/assets/9b1c588a-ab7e-448e-8b89-1bd593bf2d9c" />


### Eliminar el contenedor wordpress

<img width="1461" height="628" alt="image" src="https://github.com/user-attachments/assets/f58d9c56-cce2-4034-a589-d1629ab60c9f" />

### Crear nuevamente el contenedor wordpress
Ingresar a: http://localhost:9300/ 
recordar que a es el puerto que usó para el mapeo con wordpress

### ¿Qué ha sucedido, qué puede observar?

Al recrear el contenedor de WordPress, la publicación y la configuración del sitio permanecen.
Esto ocurre porque la información se guarda en la base de datos del contenedor MySQL, el cual no fue eliminado.

