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
