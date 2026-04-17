# Variables de Entorno
### ¿Qué son las variables de entorno?
Se utiliza para listar los archivos y directorios dentro de una ruta específica en el sistema de archivos del contenedor. Por defecto, si no se especifica ruta, lista el contenido del directorio actual (WORKDIR).

### Para crear un contenedor con variables de entorno

```
docker run -d --name <nombre contenedor> -e <nombre variable1>=<valor1> -e <nombre variable2>=<valor2>
```

### Crear un contenedor a partir de la imagen de nginx:alpine con las siguientes variables de entorno: username y role. Para la variable de entorno rol asignar el valor admin.

<img width="904" height="568" alt="Captura de pantalla 2026-04-17 a la(s) 3 26 13 p  m" src="https://github.com/user-attachments/assets/1ae22ab2-e5d7-43ce-bdda-4358a5355fc8" />

### Crear un contenedor con la imagen de mysql, mapear todos los puertos
<img width="869" height="585" alt="Captura de pantalla 2026-04-17 a la(s) 3 05 09 p  m" src="https://github.com/user-attachments/assets/a53b397d-d1e1-4488-8a39-485b50e22ba6" />

### ¿El contenedor se está ejecutando?
No se esta ejecutando

### Identificar el problema
Viendo los logs dice que no esta configurada la contraseña para el usuario root por defecto.

### Para crear un contenedor con variables de entorno especificadas
- Portabilidad: Las aplicaciones se vuelven más portátiles y pueden ser desplegadas en diferentes entornos (desarrollo, pruebas, producción) simplemente cambiando el archivo de variables de entorno.
- Centralización: Todas las configuraciones importantes se centralizan en un solo lugar, lo que facilita la gestión y auditoría de las configuraciones.
- Consistencia: Asegura que todos los miembros del equipo de desarrollo o los entornos de despliegue utilicen las mismas configuraciones.
- Evitar Exposición en el Código: Mantener variables sensibles como contraseñas, claves API, y tokens fuera del código fuente reduce el riesgo de exposición accidental a través del control de versiones.
- Control de Acceso: Los archivos de variables de entorno pueden ser gestionados con permisos específicos, limitando quién puede ver o modificar la configuración sensible.

### ¿Qué bases de datos existen en el contenedor creado?
<img width="904" height="568" alt="Captura de pantalla 2026-04-17 a la(s) 3 19 34 p  m" src="https://github.com/user-attachments/assets/f72d3184-9508-430e-b995-bed053132c5c" />
