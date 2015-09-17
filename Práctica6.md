# swap1415

# Práctica 6 : Configuración de discos en RAID

Tras añadir mediante VirtualBox 2 discos duros nuevos e iguales a una maquina virtual ya creada y configurada, procedemos a la creación del raid.

En primer lugar instalamos el mdadm con apt-get.

Despues, mediante el comando "sudo mdadm -C /dev/md0 --level=raid1 --raid-devices=2 /dev/sdb /dev/sdc", creamos el dispositivo RAID, al que despues daremos formato con "mkfs /dev/md0.

![imagen] (https://github.com/manujb90/swap1415/blob/master/Imagenes/P6/crear_raid1.png)

Despues de crear el directorio donde se montará la unidad RAID, comprobamos su estado ejecutando "sudo mdadm --detail /dev/md0:

![imagen] (https://github.com/manujb90/swap1415/blob/master/Imagenes/P6/estado_raid1.png)

	