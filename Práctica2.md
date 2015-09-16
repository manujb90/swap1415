# swap1415

# Práctica 2 : Clonar información de un sitio web

Instalamos el RSYNC mediante el comando:
	sudo apt-get install rsync
y probamos a copiar la carpeta con el contenido del servidor web con el comando:
	rsync -avz -e ssh root@maquina1:/var/www/ /var/www/

Generamos una clave para el SSH mediante el comando:
	ssh-keygen -t dsa
y a continuación la copiamos la clave:
	ssh-copy-ip -i .ssh/id_dsa.pub root@192.168.1.50

root@maquina2 ~]# ssh maquina1 -l root
![imagen] (https://github.com/manujb90/swap1415/blob/master/Imagenes/P1/ssh1.png)
	 	