# swap1415

# Práctica 5 : Replicación de bases de datos maestro-esclavos


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

Tras realizar la configuración maestro/esclavo, de la que olvidé sacar capturas, pero que es trivial siguiendo los pasos del guion, vemos con el comando SHOW SLAVE STATUS\G que la variable "Secons_Behind_Master" es distinta de "null":

![imagen] (https://github.com/manujb90/swap1415/blob/master/Imagenes/P5/show_slave.png)
	