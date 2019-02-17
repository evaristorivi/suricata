Suricata
========
<img src="https://i.ibb.co/CJxDn7g/69524480e9c7138de37a53a61d190aa0.gif" alt="vistaprevia" border="0">

Introducción
------------
Suricata es un motor de detección de amenazas de red gratuito, de código abierto, maduro, rápido y robusto.

El motor Suricata es capaz de detección de intrusión en tiempo real (IDS), prevención de intrusión en línea (IPS), monitoreo de seguridad de red (NSM) y procesamiento de pcap fuera de línea.

Suricata inspecciona el tráfico de la red utilizando un lenguaje de firmas y reglas poderosas y extensas, y tiene un potente soporte de scripts Lua para la detección de amenazas complejas.

Con formatos de entrada y salida estándar como YAML y JSON, las integraciones con herramientas como SIEMs existentes, Splunk, Logstash / Elasticsearch, Kibana y otras bases de datos se vuelven sin esfuerzo.

El rápido desarrollo impulsado por la comunidad de Suricata se centra en la seguridad, la facilidad de uso y la eficiencia.

El proyecto y el código de Suricata son propiedad y están respaldados por la Open Information Security Foundation ( OISF ), una fundación sin fines de lucro comprometida a garantizar el desarrollo y el éxito sostenido de Suricata como un proyecto de código abierto.

A) Instalación
------------
```
docker pull evaristorivi/suricata
```

Lanzar contenedor
-----------------
```
docker run -d \
    --name suricata \
    --privileged \
    --network host \
    evaristorivi/suricata \
        -i <INTERFACE>
```

Accediendo al contenedor
------------------------
```
docker exec -it suricata /bin/bash
```

