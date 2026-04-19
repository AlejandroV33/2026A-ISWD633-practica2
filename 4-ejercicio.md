## Esquema para el ejercicio
![Imagen](esquema-4-ejercicio.PNG)

### Crear la red
<img width="932" height="610" alt="Captura de pantalla 2026-04-19 a la(s) 1 28 01 p  m" src="https://github.com/user-attachments/assets/a352525c-6cb1-40f9-a950-1bc9f8883fca" />

### Crear el contenedor mysql a partir de la imagen mysql:8, configurar las variables de entorno necesarias
<img width="932" height="610" alt="Captura de pantalla 2026-04-19 a la(s) 1 30 01 p  m" src="https://github.com/user-attachments/assets/b7523587-e059-4c16-9fab-ecb69b54464e" />

### Crear el contenedor wordpress a partir de la imagen: wordpress, configurar las variables de entorno necesarias
<img width="932" height="610" alt="Captura de pantalla 2026-04-19 a la(s) 1 31 35 p  m" src="https://github.com/user-attachments/assets/586dcb51-d523-4453-92d9-ad2b0c45c248" />

De acuerdo con el trabajo realizado, en el esquema del ejercicio el puerto a es **(completar con el valor)**

Ingresar desde el navegador al wordpress y finalizar la configuración de instalación.
<img width="1624" height="1061" alt="Captura de pantalla 2026-04-19 a la(s) 1 46 59 p  m" src="https://github.com/user-attachments/assets/e0d3346a-9bb2-4b7d-b629-070dd12f13ce" />

Desde el panel de admin: cambiar el tema y crear una nueva publicación.
Ingresar a: http://localhost:9300/ 
recordar que a es el puerto que usó para el mapeo con wordpress
<img width="1624" height="1061" alt="Captura de pantalla 2026-04-19 a la(s) 1 55 58 p  m" src="https://github.com/user-attachments/assets/87576857-fcbb-493d-b19c-ac00bfc2b77a" />

### Eliminar el contenedor wordpress
<img width="1039" height="682" alt="Captura de pantalla 2026-04-19 a la(s) 1 57 15 p  m" src="https://github.com/user-attachments/assets/665deebe-f289-4dc5-8110-ae8a38ad354c" />

### Crear nuevamente el contenedor wordpress
Ingresar a: http://localhost:9300/ 
recordar que a es el puerto que usó para el mapeo con wordpress

### ¿Qué ha sucedido, qué puede observar?
Los datos de configuración y la publicación se guarda en la base de datos del contenedor srv-mysql, sin embargo parece que algo no funcion bien y wordpress intenta recuperar los datos para carga pero falla, y solo aparece una pantalla blanca sin importar cuantas veces reinicie ambos contenedores. <img width="1624" height="1061" alt="Captura de pantalla 2026-04-19 a la(s) 2 22 40 p  m" src="https://github.com/user-attachments/assets/3d04bcd1-68e0-496a-97c9-b5293a59aad2" />

