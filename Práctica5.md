# swap1415

# Práctica 4 : Comprobar el rendimiento de servidores web


![imagen] (https://github.com/manujb90/swap1415/blob/master/Imagenes/P3/prueba_haproxy.png)
En primer lugar creamos la base de datos en la maquina maestra (Maquina 1):

![imagen] (https://github.com/manujb90/swap1415/blob/master/Imagenes/P5/crear_DB.png)

Y a continuación introducimos algunos datos en esta:

![imagen] (https://github.com/manujb90/swap1415/blob/master/Imagenes/P5/crear_DB_datos.png)

Probamos a hacer una copia y vemos que efectivamente se realiza:

![imagen] (https://github.com/manujb90/swap1415/blob/master/Imagenes/P5/copia_DB.png)





Replicación de BD mediante una configuración
maestro-esclavo:


En primer lugar configuramos el mysql en el el maestro, para lo que necesitaremos editar el archivo de confiruración /etc/mysql/my.conf con las lineas que se indican en el guion.

Hacemos lo mismo en el escalvo pero poniendo el server-id a 2 y reiniciamos el servicio en ambas para aplicar los cambios. 	