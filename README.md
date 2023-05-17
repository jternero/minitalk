
# *MINITALK*  

Este proyecto es una implementación de una comunicación cliente-servidor utilizando señales en C.
El cliente y el servidor se comunican enviando y recibiendo mensajes en formato ASCII.

# El proyecto está organizado en los siguientes archivos:

Makefile: Archivo para compilar y construir el proyecto.

minitalk.h: Archivo de encabezado que contiene las declaraciones de funciones y estructuras utilizadas en el proyecto.

server.c: Archivo fuente del servidor que recibe y muestra los mensajes recibidos.

client.c: Archivo fuente del cliente que envía los mensajes al servidor.

minitalk_utils.c: Archivo fuente que contiene funciones auxiliares utilizadas por el cliente y el servidor.

server_bonus.c: Archivo fuente del servidor de bonificación que maneja múltiples clientes simultáneamente.

client_bonus.c: Archivo fuente del cliente de bonificación que permite enviar mensajes a un servidor específico.

# Compilación y ejecución
Para compilar el proyecto, ejecuta el siguiente comando:  make
Esto generará dos archivos ejecutables: server y client.

Para ejecutar el servidor, usa el siguiente comando:  ./server
El servidor comenzará a escuchar y mostrará los mensajes recibidos.

Para ejecutar el cliente y enviar un mensaje al servidor, utiliza el siguiente comando:  ./client [PID del servidor] [mensaje]

Reemplaza [PID del servidor] con el ID de proceso del servidor al que deseas enviar el mensaje y [mensaje] con el mensaje que deseas enviar.
