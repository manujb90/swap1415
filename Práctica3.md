# swap1415

# Práctica 3 : Balanceo de carga

Creamos una nueva máquina virtual para el balanceador, en la que instalaremos nginx y haproxy.

Una vez instalado nginx como se detalla en el guion, procedemos a modificar el .conf:

![imagen] (https://github.com/manujb90/swap1415/blob/master/Imagenes/P3/conf-nginx.png)

y probamos su funcionamiento una vez configurado, asegurandonos de que entra cada vez en una maquina, ya que ambas tienen elmismo peso:


![imagen] (https://github.com/manujb90/swap1415/blob/master/Imagenes/P3/prueba_balan.png)

A continuación cambiamos los pesos de las maquinas, asignandole 2 a la segunda maquina (Suponiendo en este caso que es el doble de potente que la primera, aunque sean iguales):


![imagen] (https://github.com/manujb90/swap1415/blob/master/Imagenes/P3/balanc_peso.png)

Ahora instalaremos haproxy como se detalla en el guion, procediendo despues a la modificación del archivo haproxy.cfg:


![imagen] (https://github.com/manujb90/swap1415/blob/master/Imagenes/P3/conf_haproxy.png)

y probando por último el funcionamiento de este:

![imagen] (https://github.com/manujb90/swap1415/blob/master/Imagenes/P3/prueba_haproxy.png)



	 	