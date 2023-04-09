# Use Traefik as a Reverse Proxy with cloudflare ddns

You will need to open the port 433 on your router and forward it to your server ip. (docker host)

## Demo dashboard

![traefik_demo](https://raw.githubusercontent.com/alexx855/traefik-proxy-home/master/traefik-demo.jpg)

## Create custom env file

``` bash
 cp .env.example .env
 code .env
 ```

Create your custom datasource for grafana at ./grafana/provisioning/datasources/datasource.yml

### Run the docker compose

``` bash
docker compose up -d
```

## Start the demo whoami service with the following command

``` bash
docker compose -f whoami-docker-compose.yaml up
```

## FileProvider configuration

Add any custom dynamic configuration at ./FileProvider/config.yaml
Traefik FileProvider docs <https://doc.traefik.io/traefik/providers/file/>

[![traefik_docs](https://raw.githubusercontent.com/alexx855/traefik-proxy-home/master/traefik-docs.jpg)](https://doc.traefik.io/traefik/providers/file/)
