# Docker-vuln-labs
entornos controlado diseñado para estudiantes y principiantes que desean practicar técnicas de pentesting ético y mejorar sus habilidades en ciberseguridad. Utilizando Docker y Docker Compose.



Aquí tienes un conjunto de instrucciones para agregar a tu repositorio sobre cómo instalar y ejecutar el entorno de laboratorio utilizando Docker Compose y el archivo docker-compose.yml que tienes. Estas instrucciones estarán orientadas para principiantes y estudiantes, asegurando que entiendan el proceso paso a paso.

🔐 Instrucciones de Instalación para Laboratorio de Ciberseguridad con Docker
Este repositorio contiene un laboratorio de ciberseguridad controlado que utiliza Docker y Docker Compose para configurar varios servicios y aplicaciones vulnerables. Este entorno está diseñado para que estudiantes y principiantes puedan practicar técnicas de pentesting ético en un entorno seguro.

📋 Requisitos previos
Asegúrate de tener instaladas las siguientes herramientas antes de empezar:

Docker 
Docker Compose 

Puedes verificar si Docker y Docker Compose están correctamente instalados ejecutando los siguientes comandos:
docker --version
docker-compose --version

🛠️ Pasos para la instalación
1. Clonar el repositorio

Clona este repositorio en tu máquina local:

git clone <URL_DEL_REPOSITORIO>
cd <NOMBRE_DEL_REPOSITORIO>

2. Revisar el archivo docker-compose.yml

El archivo docker-compose.yml define los servicios que se levantarán (Metasploitable2, DVWA, MySQL, etc.). Asegúrate de revisar y ajustar cualquier configuración si es necesario, aunque el archivo está listo para usarse sin cambios.

3. Levantar los servicios

Para levantar todos los servicios definidos en el archivo docker-compose.yml, simplemente ejecuta el siguiente comando:

docker-compose up -d

Este comando descargará las imágenes de Docker necesarias y ejecutará los contenedores en segundo plano

4. Verificar que los servicios estén corriendo

Puedes verificar que los contenedores estén en ejecución utilizando

docker ps -a 

------------------------------------------------------
🚧 Apagar los servicios
Cuando hayas terminado de trabajar en el laboratorio, puedes apagar todos los contenedores con el siguiente comando:

docker-compose down
Este comando detendrá y eliminará los contenedores, pero mantendrá las imágenes descargadas para que puedas reiniciar rápidamente el entorno.

🔄 Reiniciar el entorno
Si deseas reiniciar el entorno, solo tienes que ejecutar nuevamente:

docker-compose up -d

⚠️ Notas importantes
Este laboratorios estan diseñado para usarse únicamente en un entorno controlado. No expongas estos servicios a redes públicas, ya que contienen vulnerabilidades intencionales.

Si encuentras algún problema durante la instalación o la ejecución de los servicios, revisa los logs del contenedor correspondiente con el siguiente comando:

docker logs <nombre_del_contenedor>

👨‍💻 Contribuciones
Si deseas contribuir con mejoras o añadir nuevas funcionalidades a los laboratorios, no dudes en crear un pull request o abrir un issue en el repositorio.


