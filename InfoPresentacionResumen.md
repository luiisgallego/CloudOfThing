# IOT Y CLOUD 

Como ya sabréis mi presentacion trata sobre IOT y Cloud Computing y la he querido titular como Cloud of Things. No es un término elegido al azar, ya que une los dos conceptos principales y durante la investigación realizada me he encontrado con el término en varias ocasiones.

Principalmente lo que vamos a ver es una pequeña introdución para situar el contexto y luego una idea basica de que es IOT y Cloud Computing. Luego las características de esta unión y algunas posibles herramientas en el caso de que quisieramos desarrollar una aplicación cloud para iot. Además también quiero presentar los dos nuevos paradigmas que están tratando esta problematica. 



## 1 - INTRODUCCIÓN

Actualmente la cantidad de dispositivos conectados a Internet crece exponencialmente, el volumen de los datos generado por las aplicaciones de usuario en esos dispositivos aumenta cada día. En definitiva se tienen cada vez mas dispositivos conectados a Internet, tales como ordenadores, teléfonos móviles, sensores, cámaras de vigilancia, GPS, consolas de videojuegos; cada uno de ellos corriendo aplicaciones tales como redes sociales, georeferenciación, sistemas transaccionales, alertas, etc. y cada una de ellas generando datos en una amplia gama de formatos (texto, gráficos, imágenes, videos, sonidos, etc).


El primer inconveniente que se presenta en estos contextos es el almacenamiento local de los datos, además de la capacidad de procesamiento y memoria, junto con las restricciones de consumo de energía.

Esta problemática plantea la necesidad de la integración del Iot y el Cloud Computing con el fin de definir un nuevo paradigma denominado Cloud of Things. Esta unión tecnológica permitirá que el IoT aporte los medios para que el usuario interactúe mediante redes y dispositivos ubicuos. Y el Cloud permitirá el acceso a un conjunto de recursos virtualizados capaces de almacenar y procesar bajo demanda la gran cantidad de datos generada por las aplicaciones alojadas en los dispositivos.

Comentar también que muy ligado a estos dos conceptos está el de Big Data, pero por no abarcar excesivamente no vamos a tratarlo.



## 2 - CONCEPTOS 

Los avances tanto en computación móvil como dispositivos moviles, redes inalámbricas y sistemas embebidos han dado lugar al paradigma de IoT el cual consiste en una infraestructura de red global y dinámica de nodos (things) interconectados, que además son inteligentes y auto configurables. IoT permite no solo que las personas se interconecten y se comuniquen, sino que ahora también lo hacen los procesos, los datos y los objetos. 

La interacción entre los pilares de IoT establece tres tipos de conexiones: 
	- personas que se comunican con personas (P2P)
	- máquinas que se comunican con personas (M2P)
	- máquinas que se comunican con máquinas (M2M). 

Sin importar cual de estos tipos de conexiones se usan, en todos los casos se trata de una unión de múltiples tecnologías para permitir intercambiar datos entre dispositivo conectado. Todo esto se realiza con base en tecnologías de sensores, RFID, NFC y sistemas de geolocalización, que permitirán que los objetos cotidianos se conecten y se vuelvan inteligentes.


Actualmente, el 99% de los objetos que se encuentran en el mundo físico no están conectados aún a Internet, sin embargo se estima que para el año 2020 habrá 50 millones de objetos inteligentes conectados a Internet, los cuales proporcionarán billones de gigabytes de datos que deben ser almacenados, procesados e interpretados de forma eficiente. Se considera que el 90% de los datos existentes se han generado en los últimos dos años, esto está dando lugar a la Era del Exa y Zetta Byte. Este aumento en la cantidad de datos demanda un cambio de paradigma en las arquitecturas de cómputo, los algoritmos y los mecanismos de procesamiento.

En definitiva aquí es donde entra en función el Cloud Computing como sistema de apoyo para el IOT y para tratar con esa cantidad de datos.

Cloud Computing, es un modelo para permitir el acceso en red omnipresente y bajo demanda a un conjunto compartido de recursos informáticos configurables tales como, redes, servidores, almacenamiento, aplicaciones y servicios que pueden ser rápidamente aprovisionados y liberados con un mínimo de gestión esfuerzo e interacción con el proveedor o administrador de servicio.



## 3 - CARACTERÍSTICAS

IoT promete un mundo donde todo este conectado, para lograr esto es necesario: accesibilidad y conectividad ubicua, orquestación dinámica de dispositivos, óptima utilización de recursos y personalización de servicios. Pero para esto necesitamos asegurar altos niveles de disponibilidad y escalabilidad.

Pero debido a las limitaciones de los dispositivos de IoT, aspectos tales como seguridad, confiabilidad e integridad no se pueden asegurar pues no existen recursos necesarios. Por tanto, una infraestructura que integre cloud e IoT permitira: 

- Almacenamiento: Es posible alojar datos estructurados y no estructurados en múltiples formatos.
- Cómputo: Uno de los retos en ambientes IoT es la escalabilidad y el cloud lo puede proveer mediante el uso de infraestructura de altas prestaciones capaces de realizar cómputo intensivo. Aquí es donde entraría en funcionamiento el Big Data.
- Comunicación: por lo general los dispositivos de IoT usan una IP para identificarse, lo cual no es un esquema global. Para solucionar esto cloud usa la georeferenciación, que permite identificar cualquier objeto en cualquier lugar que este.
- Nuevas habilidades: El cloud resuelve parte de los problemas del IOT, además provee facilidad de acceso, facilidad de uso y costos de implementación reducidos.



## 4 - HERRAMIENTAS

Ahora para se presenta ahora una serie de herramientas con las que desarrollar aplicaciones de IOT que hagan uso del cloud. A partir de las cuales es posible desarrollar futuras aplicaciones de enfoque específico a distintos campos como las Ciudades Inteligentes o Domótica. 

### Proveedor Cloud

- AWS IoT Core es la plataforma que permite conectar dispositivos a servicios de AWS y habilitar aplicaciones para que interactúen con los terminales.

- Azure IoT Suite proporciona una colección de servicios destinados al desarrollo de plataformas IoT.

- Cloud IoT Core es el servicio que permite conectar y administrar datos desde dispositivos remotos.

Aqui podemos ver los servicios específicos de los principales proveedores de cloud, aunque también podriamos desplegar nuestras aplicaciones sin hacer uso de estos servicios específicos. De hecho comentar que Google entró más tarde en este mercado y tiene camino por recorrer ya que AWS y Azure presentan mayor madurez de arquitectura y un catálogo más amplio de servicios IoT. Según los requisitos de los clientes, se suele elegir Azure por su capacidad de integración con nubes privadas y rendimiento.



### Servidor Web (Apache, Nginx y Lighttpd)

Apache es el servidor web más utilizado a nivel mundial, es estable y robusto; su manejo de peticiones se da por medio de hilos y procesos, donde cada petición es separada en un hilo de procesamiento diferente utilizando sockets síncronos. Debido a su naturaleza síncron para aplicaciones que requieren de un tráfico considerablemente alto quizás no sea la mejor opció.

Nginx es un servidor web y proxy inverso. Gestiona las peticiones por medio de una arquitectura orientada a eventos donde las peticiones son aceptadas mediante sockets asíncronos y son procesadas en un único hilo de ejecución. Además os tiempos de respuesta son menores con Nginx respecto a Apache.

Lighttpd es un servidor HTTP cuya arquitectura es orientada a eventos. Al igual que Nginx, funciona en un solo hilo de procesamiento. Está diseñado y optimizado para ambientes de alto rendimiento con un consumo de memoria bastante reducido respecto a otros servidores web. 

---
Apache no es el más indicado para su implementación en IoT debido a su arquitectura de naturaleza bloqueante. Por su parte, Nginx y Lighttpd representan opciones muy viables, sin embargo, Nginx actúa también como un proxy inverso, lo cual añade una capa extra de seguridad entre el cliente y el servidor web, necesarios en entornos IoT como en cualquier aplicación en general.



### Protocolo de comunicación(HTTP, MQTT, WAMP,CoAP)

HTTP, no es la opción más viable para un entorno IoT ya que requiere de muchos recursos y ancho de banda. Se debe tener en cuenta que los dispositivos que usen este protocolo, tendrán limitaciones en la duración de sus baterías, memoria, ancho de banda, entre otros. 

El protocolo MQTT está diseñado específicamente para redes de dispositivos Máquina-A-Máquina (M2M) y aplicaciones móviles. Sus mensajes se transmiten en formato binario y trabaja con el modelo publicador/suscriptor, el cual funciona como una vía de comunicación de uno-a-varios clientes, lo cual es útil en IoT para el monitoreo de dispositivos remotos. Existen varios brokers que implementan el protocolo MQTT, siendo el más famoso de ellos el bróker open source Mosquitto.

El Protocolo de Mensajería de Aplicaciones Web provee dos modos de comunicación: llamadas de procedimientos remotos (RPC) (útiles para comunicaciones de uno a uno) y publicador/subscriptor (PUB/SUB) (uno a varios o de varios a uno). Aunque su medio de transmisión es por defecto WebSockets, es posible utilizar medios diferentes. Por otro lado, el modo publicador/suscriptor es utilizado en comunicaciones de uno a varios o de varios a uno. Es capaz de comunicarse de forma nativa con un navegador web sin necesidad de intermediarios. 

--- 
MQTT es la mejor alternativa por ser un protocolo concebido para ambientes con recursos restringidos.



### Framework para aplicación web

Los frameworks en tiempo real ofrecen mejores alternativas que los de arquitectura bloqueante en cuanto al manejo de grandes cantidades de peticiones concurrentes. Por tanto, debido a que IoT supone una gran cantidad de dispositivos conectados al mismo tiempo, se ha optado por analizar solo a los frameworks en tiempo real.

Node.js es un framework que utiliza un modelo no bloqueante, orientado a eventos, que lo hace ligero y eficiente. Una de sus cualidades es su capacidad nativa de trabajar con websockets. Node.js es la plataforma web más popular para aplicaciones en tiempo real y por ende es una excelente alternativa para IoT, además cuenta con una gran comunidad que desarrolla cada vez más librerías que se incorporan con facilidad en cualquier proyecto. Actualmente ya se disponen incluso de librerías IoT para open hardware.

Tornado es un framework potente y escalable escrito en Python. Es lo suficientemente robusto como para manejar un tráfico web intensivo, es fácil de configurar y puede ser utilizado para una gran variedad de aplicaciones. Tornado es capaz de manejar decenas de miles de conexiones concurrentes y está diseñado específicamente para ser un framework de alto rendimiento. 

---
Node.js es la elección más conveniente debido a su amplia gama de paquetes disponibles que pueden ser implementados para IoT. Además ya existen varias aplicaciones funcionales en Node.js como The Thing System, Node-RED, e incluso un microcontrolador llamado Tessel que funciona en su totalidad con Node.

### Base de datos

Para almacenar y procesar grandes cantidades de información, las alternativas de bases de datos relacionales podrían no satisfacer todas las necesidades requeridas. Es ahí donde las bases de datos NoSQL entran en acción debido a la flexibilidad que proporcionan al momento de almacenar y gestionar los datos, siendo esto muy importante en el ámbito de IoT.

MongoDB. La facilidad que proporciona al momento de realizar consultas a la misma es una de sus cualidades, ya que posee un conjunto de funciones con algoritmos lo suficientemente aptos para devolver los datos solicitados en consultas no tan complejas. A pesar de ser un almacén de documentos también permite realizar consultas complejas, distinguiéndose de otras bases de datos y convirtiéndose en una opción muy potente. Proporciona además, una lista cada vez mayor de características importantes  como indexación secundaria, única, compuesta, geoespacial y de texto completo.

CouchDB es una base de datos cuya arquitectura interna es bastante tolerante a fallos, es decir, cuando se produce algún error, éste se aísla en un entorno controlado y se le da tratamiento. Las consultas se basan en vistas map-reduce escritas en código JavaScript. 

--- 
CouchDB presenta inconvenientes debido a su diseño, el cual dificulta el filtrado de datos por más de un campo, un comportamiento no deseado en IoT. MongoDB es la elección más adecuada.



## INTRO FOG - EDGE COMPUTING

Con estos nuevos paradigmas se busca solventar los problemas de comunicación de datos entre los dispositivos generadores y consumidores de los mismos al acercar los centros de procesado y análisis de datos hacia ellos, reduciendo de esta forma la latencia , con lo que se mejora la experiencia del usuario y el rendimiento de las aplicaciones que hacen uso de recursos computacionales externos.

Sin embargo esta nueva arquitectura no se plantea como un sustituto de las infraestructuras Cloud tradicionales, si no como una extensión de las mismas, la potencia de cómputo, la versatilidad y las capacidades de compartición de recursos que ofrece un centro de datos cloud seguirá siendo imprescindible para muchas aplicaciones. Además aquellas aplicaciones que requieran del procesado de datos en tiempo real para responder con inmediatez a determinados eventos, o que por sus características demanden un gran consumo de ancho de banda, podrán sacar partido de la cercanía y baja latencia que ofrece un paradigma como Fog Computing para parte de sus necesidades o la totalidad de las mismas.


## 5 - FOG COMPUTING

Fog computing se considera como una extensión del paradigma de computación en nube desde el núcleo de la red hasta el borde de la red. Esta plataforma proporciona servicios de computación, almacenamiento y trabajo en red entre dispositivos finales y servidores en la nube tradicionales. Por lo general tiene tareas que pueden ser para admitir funciones de red básicas o nuevos servicios y aplicaciones que se ejecutan en un entorno de espacio aislado.



Como ya hemos comentado cada día va creciendo la producción de datos gracias a los dispositivos y sensores, pero estos no tienen los recursos de cómputo y almacenamiento para realizar análisis avanzados y tareas de aprendizaje automático. Los servidores en la nube tienen la capacidad de hacerlo, pero en ocasiones no de la manera más oportuna.

En Fog computing, el procesamiento tiene lugar en un centro de datos en un dispositivo inteligente, o en un enrutador o puerta de enlace inteligente, lo que reduce la cantidad de datos enviados a la nube. Pero estas redes complementan mas no reemplazan, la computación en la nube; esta computación permite la analítica a corto plazo, y la nube realiza análisis a largo plazo que requieren muchos recursos.



## 6 - EDGE COMPUTING

En muchos casos los tiempos de respuesta o la velocidad que requieren algunas operaciones es mayor que lo que la nube puede ofrecer. Los procesos más complejos y de gran tamaño necesitan un poder computacional cada vez más rápido y efectivo, sin poder esperar para conectarse a alguna red. Es ahí donde tenemos a Edge Computing.

Edge Computing hace referencia a cómo los procesos computacionales se realizan al interior de los dispositivos edge: aparatos IoT con capacidad de análisis y procesamiento como routers o gateways de red, la “periferia” (edge) de la red. Al procesar la información obtenida cerca de donde fue creada, sin tener que enviarla a centros de datos lejanos se reducen latencias, se consume un menor ancho de banda y se puede hacer análisis y evaluación inmediata de la información generada por los sensores y dispositivos.



Edge Computing es una red de malla de micro centros de datos que procesa o almacena datos críticos localmente y empuja todos los datos recibidos a un centro de datos central o repositorio de almacenamiento en la nube, en una superficie de menos de 30 metros cuadrados. Al alejarse de los centros de datos centrales se reduce la latencia y mejora el rendimiento general, mejorando notablemente la entrega de servicios digitales. 

Se puede definir un nodo de computación Edge como un hardware con capacidad de cómputo situado físicamente cerca de los dispositivos o equipos que hacen uso de sus recursos.

Un escenario típico puede ser el caso en el que los nodos de computación se necesitan estar físicamente cerca de las fuentes de datos, como un robot industrial o un sensor de presión de un tanque de combustible o un indicador de consumo de la red eléctrica.



## 7 - CONCLUSIÓN

La Edge Computing se refiere de forma específica a cómo los procesos computacionales se realizan en los los dispositivos IoT con capacidad de análisis y procesos como routers o gateways de red mientras que Fog Computing se refiere a las conexiones de red entre los dispositivos edge y la nube.

Hace tiempo que el OpenFog Consortium formado por Cisco, Intel, Microsoft, Dell EMD y algunas instituciones académicas trabaja en especificaciones para ese tipo de implantaciones en las que los sistemas Edge Computing, los Fog Computing y los Cloud Computing interactúan para tener un sistema aún más óptimo en cuanto a la problemática planteada.

Finalmente, en función de esto y de todo lo analizado, no cabe dudas que la integración del Iot y el cloud con el objeto de realizar un adecuado almacenamiento y procesamiento de los datos, es una opción rentable, no solo desde el punto de vista económico sino también en lo que respecta a desempeño, escalabilidad, disponibilidad y calidad de los servicios ofrecidos.



