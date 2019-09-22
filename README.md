# Criptografía y seguridad informática (86.36) - Trabajo Práctico Número 1
## Segundo Cuatrimestre 2019
### Lucas Burna (9xxxx)
### Segundo Molina Abeniacar (99306)      
#     
### Índice      
#
## Objetivo del trabajo práctico
## Introducción teórica
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
