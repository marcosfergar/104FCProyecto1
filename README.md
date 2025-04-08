# Fundamentos de contenerización


## Actividad 1. Servidor Web Simple con Nginx.


### Paso 1: Construcción de la imagen

sudo docker build -t 104fcproyecto1:1.0 .

### Paso 2. Ejecutar el contenedor en el puerto 80, 100fcproyecto1 

sudo docker run -d -p 80:80 --name 104fcproyecto1 104fcproyecto1:1.0

### Paso 3. Comprobación: http://localhost 

 
### Paso 4. Se pide modificar el fichero index.html desde el contenedor. 

docker cp index.html 104fcproyecto1:/usr/share/nginx/html/index.html

