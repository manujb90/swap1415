# swap1415

# Pr�ctica 7 : Extra septiembre. Instalaci�n y configuraci�n de NFS.


Instalamos el servicio mediante apt-get con:

sudo apt-get install nfs-kernel-server nfs-common rpcbind

A continuaci�n reiniciamos la maquina virtual para ponerlo en funcionamiento y comprobamos que efectivamente se ha instalado correctamente con "grep nfs4 /proc/filesystems":

![imagen] (https://github.com/manujb90/swap1415/blob/master/Imagenes/P6/fstab-2.png)


Fuente: http://somebooks.es/?p=5598&page=2