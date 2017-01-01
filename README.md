Dockerized http://mediagoblin.org/
==================================

[Fork of Loic Dacharys Container](https://notabug.org/dachary/mediagoblin-docker) - adds RAW image support + multi file upload

The default user is admin, password admin.


Docker Compose File
------------------------------

```
version: '2'
  services:
    mediagoblin:
      restart: always
      image: siebes/mediagoblin:latest
      volumes:
        - /etc/localtime:/etc/localtime:ro
        - /LOCAL_DIR:/var/lib/mediagoblin
      ports:
        - "PORT_YOU_WANT:80"
```


