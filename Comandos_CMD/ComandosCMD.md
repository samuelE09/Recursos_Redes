# **Comandos de Red en la Consola Windows** 

* **ipconfig:** Nos detalla la información de la configuracion del adaptador de red. IPv4/IPv6, mascara de red y puerta de enlace

* **ipconfig /all:** Muestra la informacion más amplia y detallada que ipconfig. IPv4/IPv6, mascara de red y puerta de enlace, DNS primaria y secundaria, Direccion MAC, servidor DHCP...

* **ipconfig /release:** Libera todas la IP y configuraciones del adaptador de red asignada por el DHCP

* **ipconfig /release [Nombre Adaptador]:** Libera todas la IP y configuraciones del adaptador de red que ha sido asignado por el DHCP. El nombre del adaptador permite wilcards

* **ipconfig /renew:** Solicita al DHCP que se nos asigne una IP y opciones a todos nuestros adaptadores de red

* **ipconfig /renew [Nombre Adaptador]:** Solicita al DHCP que se nos asigne una IP y opciones al adaptador de red que especifiquemos. El nombre del adaptador de red permite wildcards

* **ipconfig /displaydns:** Muestra la información almacenada sobre las resoluciones de nombres cacheados

* **Redireccion de la salida a un fichero:** Redirige la salida de comando a un fichero usando ">" Ejemplo: *ipconfig > ipconfig.txt*

* **nslookup:** Permite resolver nombres a IP y viceverse, además del servidor DNS que usamos para resolverlo. Nos permite resolver un nombre a IP o viceversa especificando el servidor DNS que queremos usar para la resolcuión de nombres. Ejemplo: *nslookup miweb.com 1.1.1.1*

* **getmac /v:** Lista las direcciones MAC de los adaptadores de red

* **netsh interface show interface:** Muestra las interfaces de Red

* **netsh interface ip show interfaces | findstr "Ip Address":** Muestra las direcciones IP filtradas que tenemos configuradas

* **netsh interface ip show dnsservers:** Muestra las direcciones Ip filtradas de los servidores DNS que tenemos configuradas

* **netsh advfirewall set allprofiles state [on/off]:** Activa / Desactiva Windowsa Firewall para todos los perfiles

* **ping:** permite saber si un host está accesible o levantado enviando 4 paquetes *ICMP*. Ejemplo: *ping 1.1.1.1*

* **ping -t:** permite saber si un host está accesible o levantado enviando ilimitados paquetes *ICMP*. Ejemplo: *ping 1.1.1.1 -t*

* **tracert:** Muestra las rutas que toma los paquetes para llegar a su destino y lo lento/rápido que van. Ejemplo: tracert *google.com*

* **tracert -d:** Lo mismo que tracert pero más rápido porque no hace resolución de nombres.

* **netstat:** Muestra la información de lo que nos hemos conectado y lo que se ha conectado a nosotros.

* **netstat -af:**  Muestra los puertos que tenemos abiertos escuchando conexiones.

* **route print:***  Muestra todas las rutas que tenemos configuradas.

* **route add:**  Añade rutas estáticas para definir cómo nuestro equipo debe comunicarse a determinadas redes.

* **route delete:**  Lo contrario a route add, borra rutas.

