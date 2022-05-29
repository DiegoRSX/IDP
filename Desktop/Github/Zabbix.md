 # <center>**Monitorización con Zabbix.**
##Creamos primero las máquinas que usaremos, una ubuntu y una windows.

Máquina 1;

Ubuntu

![Imagen1](imagenes/Captura.PNG)

Máquina 2;

Windows

![Imagen2](imagenes/WIndows.PNG)

Y las conectamos mediante "Red NAT".

![Imagen3](imagenes/Rednat.PNG)

Y le haremos un ping al cliente.

![Imagen4](imagenes/ping.PNG)

Descargamos el Zabbix desde el repositorio.

![Imagen5](imagenes/Descarga.PNG)

Y lo instalamos.

![Imagen6](imagenes/instalacion.PNG)

Instalamos el paquete descargado antes:

![Imagen7](imagenes/descomprimir.PNG)

Actualizamos los repositorios.

![Imagen8](imagenes/actualizar.PNG)

Instalamos los paquetes necesarios para el servidor Zabbix.

![Imagen9](imagenes/instalaciondepaquetes.PNG)

Conectamos el servidor con la base de datos.

![Imagen10](imagenes/conectarbasededatos.PNG)

Creamos la base de datos.

![Imagen11](imagenes/creacionbasededatos.PNG)

Creamos al usuario Zabbix con contraseña password y le damos los privilegios sobre la base de datos Zabbix;

![Imagen12](imagenes/privilegios.PNG)

Cerramos mysql

![Imagen13](imagenes/cerrarmysql.PNG)

Importamos el esquema incial y los datos, utilizando la contraseña antes creada:

![Imagen14](imagenes/importarelesquema.PNG)

En la configuración nos va a pedir los requisitos.

![Imagen15](imagenes/instalacionzabbixpagina.PNG)

Nos aseguramos de que esté todo en “OK”.
Y configuramos la base de datos.

![Imagen16](imagenes/requisitoszabbix.PNG)

Y en los detalles del servidor, le pondremos de nombre, “Zabbix”.

![Imagen17](imagenes/zabbixserverdetails.PNG)

Y nos dará un resumen de la configuración.

![Imagen18](imagenes/prerrequisitoszabbix.PNG)

Y procederemos a la finalización.

![Imagen19](imagenes/finalzabbix.PNG)

Después nos pedirá loguearnos con nuestro usuario y contraseña definidos anteriormente.
Usuario: Admin 
Contraseña: Zabbix
Y veremos la interfaz.

![Imagen20](imagenes/dashboardzabbix.PNG)

Ahora pasaremos a crear un “Host” para monitorizar.

![Imagen21](imagenes/crearhostzabbix.PNG)

Y le daremos arriba a la derecha, donde nos pone “Create Host”.

![Imagen22](imagenes/createhost.PNG)

Entraremos y rellenamos los apartados.

![Imagen23](imagenes/conexionconmaquinacliente.PNG)

En “groups” le daremos a seleccionar y elegiremos el “Name” para seleccionarlo todo.

En “agents interfaces” le daremos a “add” para añadir un nuevo agente.

Y le pondremos la ip asignada a nuestra otra máquina.

![Imagen24](imagenes/conexionconmaquinacliente.PNG)

Posterior a esto, nos iremos a “templates”, situado en la barra de herramientas arriba y vamos a buscar en “seleccionar” hasta que encontremos “template Linux”.

![Imagen25](imagenes/templateszabbix.PNG)

Y le daremos a “Add” y posterioemente a “update”.

Nos vamos a “Monitoring” y pulsamos en “Graph” para dirigirnos a “Hosts” y pulsar el nombre del Host que le dimos anteriormente.

Ahora vamos a la máquina cliente, y nos descargamos el “agente zabbix” y realizamos la conexión para que esta se establezca con nuestro servicio.

![Imagen26](imagenes/agentezabbix.PNG)

Continuamos con la instalación.

![Imagen27](imagenes/instaladorcompletadoagentezabbix.PNG)

Y desactivamos el firewall de red.

![Imagen28](imagenes/desactivacionfirewall.PNG)

Posteriormente, iremos a la página y veremos que nos empezará a actualizar la información en los parámetros y después en la gráfica.

![Imagen29](imagenes/graficaclientezabbix.PNG)

Y vamos a “dashboard” para dirigirnos a “all dashboard” y vamos abajo del todo para ver el rendimiento de nuestro sistema.

![Imagen30](imagenes/rendimientoclientezabbix.PNG)

# Rendimiento de Red.

Y para hacer la administración de rendimiento red, iremos a “hosts”, seleccionaremos cualquiera de los dos, Zabbix server que el rendimiento lo proporcionará la propia máquina servidor o Windows-pc que lo proporcionará el Windows.

![Imagen31](imagenes/webzabbix.PNG)

Y seleccionamos uno.

Y pinchamos en Web.

Y arriba derecha, nos dirigimos a “Create Web scenario” y aquí rellenamos el nombre y nueva aplicación con los datos que queramos.

![Imagen32](imagenes/hostwebzabbix.PNG)

Iremos entonces a la gráfica web y nos empezará a medir el rendimiento.

![Imagen33](imagenes/paginahostzabbix.PNG)

Y lo rellenamos con los datos que necesitemos.

Le daremos a “Add” y por último, nos iremos a “Dashboard” > “Web” y dándole a “Zabbix frontend” en mi caso, accederemos a la monitorización web.

![Imagen34](imagenes/rendimientowebzabbix.PNG)
























