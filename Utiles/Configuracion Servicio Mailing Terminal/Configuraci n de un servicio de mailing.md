# Configuración de un servicio de mailing

Para poder enviar correos desde la terminal necesitamos contar con algunas utilidades en nuestra computadora.

La primera de ellas es [postfix](https://es.wikipedia.org/wiki/Postfix), un servidor de correo que se encargará de las tareas de comunicación con los servidores de destino.

En esta lectura asumiré que estás trabajando con alguna versión de Ubuntu, si no es así, los comandos podrían variar ligeramente.

Abre una terminal y asegúrate de tener tu sistema de paquetes al día usando el comando sudo apt update.

A continuación instala postfix utilizando el comando: sudo DEBIAN_PRIORITY=low apt install postfix.

Te encontrarás con una pantalla como esta:

![Configuraci%20n%20de%20un%20servicio%20de%20mailing/Untitled.png](Configuraci%20n%20de%20un%20servicio%20de%20mailing/Untitled.png)

Selecciona “Sitio de Internet” y dale “Aceptar”.

Te encontrarás con una pantalla como esta:

![Configuraci%20n%20de%20un%20servicio%20de%20mailing/Untitled%201.png](Configuraci%20n%20de%20un%20servicio%20de%20mailing/Untitled%201.png)

Dale aceptar y pasarás a una pantalla como esta:

![Configuraci%20n%20de%20un%20servicio%20de%20mailing/Untitled%202.png](Configuraci%20n%20de%20un%20servicio%20de%20mailing/Untitled%202.png)

Ingresa aquí tu dirección de correo electrónico.

Dale aceptar y verás lo siguiente:

![Configuraci%20n%20de%20un%20servicio%20de%20mailing/Untitled%203.png](Configuraci%20n%20de%20un%20servicio%20de%20mailing/Untitled%203.png)

Dale aceptar y continúa:

![Configuraci%20n%20de%20un%20servicio%20de%20mailing/Untitled%204.png](Configuraci%20n%20de%20un%20servicio%20de%20mailing/Untitled%204.png)

Responde “No” y avanza a:

![Configuraci%20n%20de%20un%20servicio%20de%20mailing/Untitled%205.png](Configuraci%20n%20de%20un%20servicio%20de%20mailing/Untitled%205.png)

Dale aceptar. Sigue con:

![Configuraci%20n%20de%20un%20servicio%20de%20mailing/Untitled%206.png](Configuraci%20n%20de%20un%20servicio%20de%20mailing/Untitled%206.png)

Acepta y continúa:

![Configuraci%20n%20de%20un%20servicio%20de%20mailing/Untitled%207.png](Configuraci%20n%20de%20un%20servicio%20de%20mailing/Untitled%207.png)

Aceptar.

![Configuraci%20n%20de%20un%20servicio%20de%20mailing/Untitled%208.png](Configuraci%20n%20de%20un%20servicio%20de%20mailing/Untitled%208.png)

Selecciona “Todos” y da “Aceptar”.

Con eso finalizará el asistente para la configuración de postfix y la instalación habrá finalizado.

Instala las utilidades de correo con el comando:

sudo apt install mailutils

Y ahora sí, tienes todo lo que necesitas para enviar correos desde la terminal.

Puedes probarlo usando el comando:

echo “Hola Mundo!” | mail -s “Testing” TU_EMAIL

Revisa tu correo (no olvides revisar la bandeja de no deseados!) y ya podrás enviarle un saludo a todos tus conocidos sin pasar por Gmail, Outlook ni nada parecido. 😃