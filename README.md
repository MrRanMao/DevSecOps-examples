# DevSecOps-examples

## Usage

If you want to use traefik, start the traefik container first and create a .env file in every subfolder you use containing the following

```
DEFAULT_NETWORK=traefik-network
DOMAIN=yourdomain.home
```

Depending on the container, you might have to create an .env file and fill in variables for the container to work (i.e. to set up export folder) even if you don't use traefik.

If you don't want to use traefik, comment the labels/networks and uncomments the ports to use plain docker.


Run a docker-compose file

```
docker-compose up -d
```

Stop

```
docker-compose down
```