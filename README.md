# Ultraviolet App - Docker
Docker images for hosting Ultraviolet and its front-end on Docker.

Docker Hub repository: https://hub.docker.com/r/diffusehyperion/ultraviolet

Also available in Github Packages: https://github.com/DiffuseHyperion/Ultraviolet-App-docker/pkgs/container/ultraviolet

...I know that there is already an existing Docker image in Ultraviolet-App, but this image is:
  - based on a more official image (node:18-alpine)
  - ignores unnecessary files
  - isn't ridiculously obsecure (to be completely honest, i had no idea an [official image](https://hub.docker.com/r/np22jpg/ultraviolet-node) existed until I was writing this readme lol)

# Usage

Example `docker run` usage:
```
docker run -v "80:80" -d diffusehyperion/ultraviolet:latest
```

Example `docker-compose.yml` usage:
```
version: '2'
services:
  ultraviolet:
    image: diffusehyperion/ultraviolet:latest
    restart: unless-stopped
    ports:
      - "80:8080"
```

Works with reverse proxies too! I recommend using [Nginx Proxy Manager](https://nginxproxymanager.com/).

# Original description

<p align="center"><img src="https://raw.githubusercontent.com/titaniumnetwork-dev/Ultraviolet-Static/main/public/uv.png" height="200"></p>

<h1 align="center">Ultraviolet-App</h1>

The deployable all-in-one bundle for Ultraviolet, a highly sophisticated proxy used for evading internet censorship or accessing websites in a controlled sandbox using the power of service-workers and more!

## Deployment

[![Deploy to Heroku](https://binbashbanana.github.io/deploy-buttons/buttons/remade/heroku.svg)](https://github.com/titaniumnetwork-dev/Ultraviolet-App/wiki/Deploy-to-Heroku)
[![Run on Replit](https://binbashbanana.github.io/deploy-buttons/buttons/remade/replit.svg)](https://github.com/titaniumnetwork-dev/Ultraviolet-App/wiki/Run-on-Replit)
[![Deploy on Railway](https://binbashbanana.github.io/deploy-buttons/buttons/remade/railway.svg)](https://github.com/titaniumnetwork-dev/Ultraviolet-App/wiki/Deploy-on-Railway)
[![Remix on Glitch](https://binbashbanana.github.io/deploy-buttons/buttons/remade/glitch.svg)](https://github.com/titaniumnetwork-dev/Ultraviolet-App/wiki/Remix-on-Glitch)
[![Deploy to Koyeb](https://binbashbanana.github.io/deploy-buttons/buttons/remade/koyeb.svg)](https://github.com/titaniumnetwork-dev/Ultraviolet-App/wiki/Deploy-to-Koyeb)

If you are deploying to an alternative service or to a server, refer to [Deploy via terminal](https://github.com/titaniumnetwork-dev/Ultraviolet-App/wiki/Deploy-via-terminal).

Additional information such as [customizing your frontend](https://github.com/titaniumnetwork-dev/Ultraviolet-App/wiki/Customizing-your-frontend) can be found on the [wiki](https://github.com/titaniumnetwork-dev/Ultraviolet-App/wiki).
