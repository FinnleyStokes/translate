"""Un minorista de moda europeo se ha convertido en la última marca de renombre en exponer datos person
ales de millones de sus clientes después de configurar mal una base de datos en la nube.Los investig
adores de vpnMentor descubrieron el servidor Elasticsearch sin cifrar el 28 de junio y la empresa ma
triz BrandBQ finalmente lo aseguró alrededor de un mes después, el 20 de agosto.El minorista con sed
e en Cracovia opera tiendas físicas y en línea en Europa del Este, en: Polonia, Rumania, Hungría, Bu
lgaria, Eslovaquia, Ucrania y la República Checa. Sus principales marcas son Answear y WearMedicine.
com.Entre los mil millones de entradas en la base de datos expuesta, 6,7 millones de registros relac
ionados con clientes en línea, con cada entrada con información de identificación personal (PII), in
cluidos nombres completos, direcciones de correo electrónico y de casa, fechas de nacimiento, número
s de teléfono y registros de pago (aunque no la tarjeta detalles).50.000 registros adicionales relac
ionados con contratistas locales en determinadas jurisdicciones incluían información adicional, como
 números de IVA e información de compra. La base de datos también contenía registros de llamadas a l
a API de la aplicación móvil de Answear, exponiendo la PII de 500.000 usuarios de la aplicación de A
ndroid y un número desconocido que descargaron la versión de iOS, afirmó vpnMentor.Los datos expuest
os podrían haber proporcionado a los ciberdelincuentes una fuente útil de PII para lanzar ataques de
 phishing convincentes y fraude de identidad, agregó.¿Qué es Elasticsearch?Elasticsearch es una plat
aforma de análisis y búsqueda de código abierto distribuida que se ejecuta en el software Lucene. El
 motor de «Búsqueda como servicio» se utiliza para el registro y el análisis de registros, la extrac
ción y combinación de datos públicos y la búsqueda de texto completo en más de 3000 empresas, inclui
das Adobe y Cisco. Elasticsearch y sus servicios hermanos Log-stash y Kibana forman la pila Elastic.
 Esta colección de servicios es inmensamente popular para administrar conjuntos de datos grandes y d
iversos debido a su capacidad de respuesta en tiempo real y su alta escalabilidad.Elasticsearch trab
aja con datos no estructurados de varias ubicaciones y luego los almacena e indexa. Esto permite una
 mejor capacidad de búsqueda, especialmente porque los usuarios pueden personalizar sus índices y ma
pas específicos según las necesidades de su organización. Elasticsearch también pone a disposición e
normes volúmenes de datos.¿Cómo ocurren las infracciones de Elasticsearch?Los grupos de búsqueda elá
sticos mal configurados y desprotegidos pueden ser descubiertos y explotados por actores malintencio
nados que buscan en la web. Una herramienta común para descubrir bases de datos expuestas es Shodan,
 que busca dispositivos y puertos conectados a Internet. Una búsqueda superficial en Shodan para los
 puertos predeterminados 9200 y 9300 de Elasticsearch revela miles de resultados, algunos de los cua
les probablemente quedarán desprotegidos. Desde allí, los actores malintencionados pueden usar la fu
nción de línea de comandos curl para ubicar y explorar los clústeres de Elasticsearch expuestos. Una
 vez que un atacante descubre datos confidenciales dentro de un clúster expuesto, pueden exfiltrarlo
s para una gran variedad de usos maliciosos. Las herramientas similares a Shodan que también se pued
en usar para buscar clústeres de Elasticsearch expuestos incluyen Censys y LeakIX. Los clústeres exp
uestos ocurren cuando los usuarios no habilitan los protocolos de seguridad integrados dentro del ki
t de herramientas de Elastic o configuran incorrectamente sus bases de datos. Por ejemplo, en una ex
posición de julio de 2019 de 90 millones de registros de datos, el clúster de Elasticsearch navegó a
 la «página de creación de patrón de índice» cuando se accede en un navegador. A partir de ahí, los 
actores malintencionados podrían explorar dos bases de datos que contienen el almacenamiento masivo 
de información confidencial."""