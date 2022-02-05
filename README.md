# 6.3.-Curso-de-fundamentos-en-AWS-cloude

_____________________________________________________________________
![](https://static.platzi.com/media/courses/OG-Fundamentos-AWS-Cloud.png)
_____________________________________________________________________
### Introducción al documento
_____________________________________________________________________
El contenido de este documento esta basado en el curso del mismo nombre dictado por Mauro Parra Miranda en Platzi.

**Table of Contents**

[TOCM]

[TOC]

# 1. ¿Qué es el cómputo en la nube?

  - En AWS el cómputo en la nube trata de los siguiente
  - Sitios Web, una sola computadora corriendo un solo stack de programación cómo LAMP, XAMPP, entre otros.
  - Respaldos y recuperación, incluso de sistemas operativos completos.

  - Archivos Permanentes, también puedes guardar archivos estáticos como fotografías o documentos.

  - DevOps, no solo tenemos automatización en el release de los proyectos, también cuentas con alta disponibilidad o respaldos automatizados en diversos lugares del mundo.

  - Análisis Masivos

  - Cómputo Serverless, en lugar de preocuparte por la cantidad de computadoras o cómo y cuándo va a escalar tu servicio puedes programar tu aplicación con microservicios mientras que AWS se encarga de darte los elementos necesarios.

  - Cómputo de Alto Rendimiento, levanta tus servidores sólo cuando tu aplicación lo necesita.

  - Internet of Things.

  - Aplicaciones Empresariales.

  - Distribución de media.

  - Servicios móviles.

  - Cómputo científico.

  - E-commerce.

  - Ambientes Híbridos.

  - Blockchain.

Ventajas de AWS:


  - Cero inversión inicial, muchos servicios son gratis el primer año

  - Usa lo que necesites, apaga lo que no

  - Crece tanto como sueñes

  - Velocidad cuando la necesitas

  - Si no lo usas, no lo pagas

  - Cobertura mundial
  
 # 2. ¿Cómo puedo empezar a usar AWS?
 
 Para crear tu cuenta de AWS debes entrar a aws.amazon.com, recuerda que para crear tu contraseña puedes usar passwordsgenerator.net.

AWS dispone de dos programas que permiten a los clientes trasladar sus enseñanzas y esfuerzos de investigación a la nube y de este modo innovar más rápidamente y con un menor costo. Para aplicar a las becas de AWS entra a aws.amazon.com/es/grants.

Cuando tengas tu cuenta registrada, entra a console.aws.amazon.com y tendrás acceso a la consola de amazon con todos los servicios disponibles.

**Lecturas recomendadas**
https://passwordsgenerator.net/
https://aws.amazon.com/es/
https://aws.amazon.com/es/grants/

# 3. Introducción a la oferta de servicios de AWS y sus aplicaciones

Los servicios en AWS se dividen en:

Compute.
Storage.
Database.
Migration & Transfer.
Networking & Content Delivery.
Developer Tools.
Robotics.
Blockchain.
Satellite.
Management & Governance.
Media Services.
Machine Learning.
Analytics.
Security, Identity, & Compliance.
Mobile.
AR & VR.
Application Integration.
AWS Cost Management.
Customer Engagement.
Business Applications.
Desktop & App Streaming.
Internet Of Things.
Game Development.

**Introducción a la oferta de AWS y sus interacciones**

# 4. Ejemplo de arquitectura con Elastic Beanstalk
 Conceptos importantes vistos en la clase:

	-AWS Elastic Beanstalk: es un servicio de ASW que se utiliza para implementar y escalar servicios y aplicaciones web desarrolladas en JAVA, .NET, PHP, Node.js, Python, Go, entre otros, en servidores familiares como Apache y Nginx. Además se encargará de administar de manera automática la implementación, el aprovisionamiento de la capacidad, el equilibrio de la carga y el escalado de nuestra aplicación.

	-CloudWatch: es un servicio de monitorieo y administración creado para desarrolladores, operadores de sistemas, entre otros. El servicio ofrece datos e información procesable para monitorear las aplicaciones, comprender cambios de rendimiento que afectan al sistema, optimizar recursos y lograr una vida unificada del estado de las operaciones.

# 5. ¿Qué es EC2?

EC2 es un conjunto de máquinas virtuales en AWS (Amazon Web Services) que puedes utilizar para ejecutar tus propias aplicaciones, tanto de calidad como desarrollo o incluso producción.

**Características de EC2 en AWS**
	-Instancias. Máquinas virtuales con diversas opciones de Sistema Operativo, vCPU, RAM y Disco Duro, entre otros.

	-Seguridad. Generación de llaves únicas para conectarte a tu máquina Linux o Windows de forma segura. Es posible generar diferentes llaves o claves para diversas máquinas.

	-Espacio. Diversas opciones de espacio en disco duro y es virtualmente infinito. Puedes anexar recursos en cualquier momento, si lo necesitas.

	-Redundancia. Es posible tener diversas copias de la misma máquina en diversas regiones geográficas.

	-Firewall. Puedes controlar desde dónde te puedes conectar a la máquina y a través de qué puertos. Además, es posible hacer modificaciones en términos de servicios y es muy fácil crear las reglas del firewall.

	-Direcciones IP estáticas. Puedes optar por comprar una IP pública estática para que siempre puedas poner la última versión o la última máquina en esa IP.

	-Respaldos. Puedes respaldar toda la máquina (ambiente, sistema operativo) cada vez que lo necesites. Además, los respaldos los puedes mover a diferentes regiones y tener múltiples copias disponibles.

	-Escalable. Es posible incrementar o disminuir los recursos de la máquina (más vCPUs, más RAM, entre otros) cuando lo necesites.

	-Migración de snapshot. Puedes copiar un snapshot a otras regiones, en caso de que algo suceda en la que estás trabajando o para agilizar la conexión desde otros lugares.

Recuerda que puedes consultar la documentación oficial de EC2 AWS en: https://docs.aws.amazon.com/es_es/AWSEC2/latest/UserGuide/concepts.html

# 6. Creando una instancia de EC2

Al momento de crear la instancia EC2 en mi cuenta siguiendo los pasos descritos en esta clase, tuve problemas por que no se podia conectar a traves de SSH. Despues de un tiempo de investigacion encontre este manual de ayuda en donde siguiendo todos los pasos pude configurar exitosamente. Espero les sea de ayuda a alguien que pase por la misma situacion que yo.

https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/TroubleshootingInstancesConnecting.html

# 7.  Conectándonos a nuestra instancia desde Windows
Sistemas UNIX como Mac y Linux traen por defecto una terminal predeterminada que funciona perfecto para conectarte por SSH (secure shell) a nuestras instancias en AWS. Sin embargo, en Windows no hay alternativas nativas que funcionen tan bien, así que puedes usar MobaXterm, un software que te ayudara a conectarnos a nuestras instancias, ademas de muchos otros beneficios.

Recuerda que eres tienes las siguientes responsabilidades:

	-Updates: Con las instancias, nosotros somos totalmente responsables de la actualización de OS
	-Respaldos: Nuestra instancia no se respaldará sola, tendremos que hacerlo nosotros.
	-Restauración snapshot: Podemos hacer respaldos antes de hacer grandes cambios para poder hacer rollback del Sistema en caso necesario.
Lecturas recomendadas

MobaXterm free Xserver and tabbed SSH client for Windows

https://mobaxterm.mobatek.net/

# 8. Conectándonos a nuestra instancia desde Linux

# 9. Conectándonos a nuestra instancia desde OSX

# 10. Subiendo un proyecto: Clonando un repositorio de GitHub a nuestra Instancia de EC2

Para clonar repositorios desde tu instancia de AWS necesitas instalar git:

# Permisos de super usuario
sudo su
# Instalación de git
yum install git
Teniendo git instalado ya podemos clonar el repositorio que necesitemos:

git clone [URL_DEL_PROYECTO]
En el siguiente link vas a encontrar el repositorio con el que vamos a trabajar en la clase: https://github.com/mauropm/aws-platzi-python.
___________________
les comparto un vídeo de como programar la instancia para que se apague y se prenda en determinado periodo de tiempo, ya que somos muchos que usamos el servicio free me parece vital optimizar los tiempos de conexión

https://www.youtube.com/watch?v=xWnlCxvojQw

# 11. Subiendo un proyecto Clonando un repositorio de GitHub a nuestra Instancia de EC2

Ahora que clonamos nuestro repositorio, vamos a instalar las dependencias necesarias para que funcione. El proyecto que trabajamos en clase sólo necesita una dependencia:

- Permisos de super usuario
sudo su
- Instalación de flask
pip install flask
Con las dependencias instaladas podemos correr nuestro servidor, en el caso de nuestro proyecto es con el siguiente comando:

python app.py
Para acceder por internet a nuestro servidor tenemos que buscar nuestra instancia de EC2 y copiar la IP pública, pero no es suficiente. Debemos entrar a Security Groups, Inbound y añadir una regla Custom TCP Rule, escribe el puerto en el que corre tu servidor (que para nuestro proyecto es el 5000) y en la opción Source elije Anywhere.

Recuerda que para encontrar tu IP pública puedes entrar a whatismyip.com.

Lecturas recomendadas

What Is My IP? Shows your real IP - IPv4 - IPv6 - WhatIsMyIP.com®

https://www.whatismyip.com/


# 12. ¿Qué es Lambda y Serverless?

Lambda es un proyecto de AWS muy relacionado con el concepto de Serverless, dejar la administración de tus servidores en manos de Amazon para solo encargarte de las funciones de código que ejecutara tu aplicación.

¿Qué son?
Imagina lambda como un lugar donde puedes ejecutar funciones de tu código.

Serverless
No existe un servidor como vimos en EC2, es decir, solo está el código en lamba y AWS se encarga de ejecutarlo cuando necesites.

Lenguajes soportados
Puedes programar funciones lamba en Nodejs (JavaScript), Python, Java (8), C# (.Net Core) y Go.

Recuerda tener en cuenta los siguientes puntos:

	-Memoria: Mínima de 128MB, máxima 3000MB con incrementos de 64MB.
	-Límites de ejecución y espacio: Puedes correr tu aplicación hasta 300 segundos y tienes un /tmp limitado a 512MB.
	-Ejecución paralela: Esta limitada a 1000 ejecuciones concurrentes (a un mismo tiempo), no tiene límite en ejecuciones secuenciales (una detrás de otra).
	-Ventajas de Lambda:

	-Seguridad: Al ser una infraestructura compartida, no tienes que preocuparte de seguridad: AWS maneja todo.
	-Performance: AWS está monitoreando constantemente la ejecución de tus funciones y se encarga de que siempre tenga el mejor performance.
	-Código aislado: Tu código, aún estando en una infraestructura compartida, corre en un ambiente virtual exclusivo, aislado de las demás ejecuciones lamba.
	-Recuerda que AWS te regala 1 millón de peticiones lamba gratis el primer año.
