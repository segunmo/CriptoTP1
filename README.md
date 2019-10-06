# Criptografía y seguridad informática (86.36) - Trabajo Práctico Número 1
## Segundo Cuatrimestre 2019
### Lucas Burna (99608)
### Segundo Molina Abeniacar (99306)      
#     
## Objetivo del trabajo práctico
El objetivo del presente trabajo practico es el de realizar un analisis criptografico basico y el posterior ataque a las vulnerabilidades que presentan las redes WEP(Wired Equivalent Privacy). Mediante el presente informe se dan a conocer los pasos realizados para la obtención de claves de Wifi que presentan las redes WEP.
## Introducción teórica
Las redes WEP, tal como lo indica su nombre Wired Equivalent Privacy, surgieron como el equivalente inalámbrico de las redes cableadas, proporionando el mismo nivel de seguridad. El estándar 802.11 especifica su capacidad de cifrado.
	El protocolo de seguridad está basado en RC4 y utiliza 64 o bien 128 bits, donde 24 de ellos pertenecen al vector de inicializacion (IV). Para poder descifrar la clave  contenida en los 40 o 104 bits correspondientes, estos 24 bits forman parte de los paquetes enviados, pues ambos emisor y receptor deben conocer los IV ( que se envían sin cifrar). Además, los patrones de generación de vectores predecibles y por lo tanto vulnerables. 
## Documentación

Para la realización de este trabajo práctico necesitaremos herramientas de análisis de redes WiFi. El sistema operativo Kali, basado en el kernel de Linux provee estas herramientas como así también otras que son relevantes a la materia. Por cuestiones de seguridad y practicidad decidimos instalar el sistema operativo en una máquina virtual. En este caso optamos por Virtualbox, una opción de código abierto y gratis.    


Procedemos a instalar VirtualBox desde [su página oficial](https://www.virtualbox.org/wiki/Downloads) para un host Windows 10.    


![InstalamosVirtualBox][InstalamosVirtualBox]

Comprobamos el checksum   
![ComprueboChecksum][ComprueboChecksum]

Luego descargamos la imagen de Kali para Virtualbox desde (su página oficial)[https://www.offensive-security.com/kali-linux-vm-vmware-virtualbox-image-download/]   y verificamos el checksum
![DescargamosKali][DescargamosKali]   
![ChecksumKali][ChecksumKali]   

Abrimos VirtualBox
![AbrimosVirtualBox][AbrimosVirtualBox]     


Importamos la imagen de Kali en VirtualBox
![ImportamosKali1][ImportamosKali1]   
![ImportamosKali2][ImportamosKali2]   
![ImportamosKali3][ImportamosKali3]   
![ImportamosKali4][ImportamosKali4]   

Intentamos correr Kali en VirtualBox pero nos encontramos con el siguiente error:
![ErrorVB][ErrorVB]   

Descargamos el paquete necesario    
![DescargamosPaquete][DescargamosPaquete]


Lo instalamos   
![InstalamosPaquete][InstalamosPaquete]


Corremos Kali   
![CorremosKali1][CorremosKali1]
![CorremosKali2][CorremosKali2]
![CorremosKali3][CorremosKali3]   

 En un primer intento tratamos de crackear la red WEP, pero no se detectó su presencia debido al uso de Kali dentro de un entorno dado por una máquina virtual, con lo cual el sistema operativo primario no permite el uso de la placa de red propia de la notebook
 ![Kali_placa_red_necesaria][Kali_placa_red_necesaria]
Luego de adquirir una placa de red USB, tal como se muestra en la imagen
 ![kali_red_disponible][kali_red_disponible]
procedimos a utilizar las herramientas incluidas en Kali para crackear la contraseña de la red WEP.

## Conclusiones



[InstalamosVirtualBox]: Imagenes/InstalamosVirtualBox.png
[ComprueboChecksum]: Imagenes/ComprueboChecksum.png
[DescargamosKali]: Imagenes/DescargamosKali.png
[ChecksumKali]: Imagenes/ChecksumKali.png
[AbrimosVirtualBox]: Imagenes/AbrimosVirtualBox.png
[ImportamosKali1]: Imagenes/ImportamosKali1.png
[ImportamosKali2]: Imagenes/ImportamosKali2.png
[ImportamosKali3]: Imagenes/ImportamosKali3.png
[ImportamosKali4]: Imagenes/ImportamosKali4.png
[ErrorVB]: Imagenes/ErrorVB.png
[DescargamosPaquete]:Imagenes/DescargamosPaquete.png
[InstalamosPaquete]: Imagenes/InstalamosPaquete.png
[CorremosKali1]: Imagenes/CorremosKali1.png
[CorremosKali2]: Imagenes/CorremosKali2.png
[CorremosKali3]: Imagenes/CorremosKali3.png
[Kali_placa_red_necesaria]: Imagenes/Kali_placa_red_necesaria.png
[kali_red_disponible]: Imagenes/kali_red-_disponible.png
