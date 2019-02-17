Suricata
========

Introducción
------------
Suricata es un motor de IDS, IPS y NSM de red.

Instalación
------------
```

git clone https://github.com/evaristorivi/suricata
cd suricata
docker build -f docker/Dockerfile -t suricata:latest .


docker run -d \
    --name suricata \
    --privileged \
    --network host \
    suricata:latest \
        -i <INTERFACE>
```

Accediendo al contenedor
------------------------
```
docker exec -it suricata /bin/bash
```
