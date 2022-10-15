# Traefik with Docker and File providers
![traefik_demo](https://raw.githubusercontent.com/alexx855/traefik-proxy-home/master/traefik-demo.jpg)

## Create custom env file
``` bash
 cp .env.example .env
 code .env
 ```

## Run the traefik compose
``` bash
docker-compose up -d
```

## Start the demo whoami service with the following command:
``` bash
docker-compose -f whoami-docker-compose.yaml up
```

## Add any custom dynamic FileProvider configuration
Traefik FileProvider docs https://doc.traefik.io/traefik/providers/file/

[![traefik_docs](https://raw.githubusercontent.com/alexx855/traefik-proxy-home/master/traefik-docs.jpg)](https://doc.traefik.io/traefik/providers/file/)

