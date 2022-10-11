# Traefik with the Docker provider
## Create custom env file
``` bash
 cp .env.example .env
 code .env
 ```

## Run the traefik compose
``` bash
docker-compose up -d
```

## Start the whoami service with the following command:
``` bash
docker-compose up -d whoami
```

## Add your custom FileProvider configuration
https://doc.traefik.io/traefik/providers/file/

