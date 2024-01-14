# cloudflare-docker-proxy

![deploy](https://github.com/ciiiii/cloudflare-docker-proxy/actions/workflows/deploy.yaml/badge.svg)

> If you're looking for proxy for helm, maybe you can try [cloudflare-helm-proxy](github.com/ciiiii/cloudflare-helm-proxy).

## Deploy
[![Deploy to Cloudflare Workers](https://deploy.workers.cloudflare.com/button)](https://deploy.workers.cloudflare.com/?url=https://github.com/nbtca/cloudflare-docker-proxy)

1. fork this project
2. modify the link of the above button to your fork url
3. click the button, you will be redirected to the deploy page

## Use

We provide proxy for docker hub and github container registry.

   ```javascript
   const routes = {
     "docker.mirror.nbtca.space": "https://registry-1.docker.io",
     "ghcr.mirror.nbtca.space": "https://ghcr.io",
   };
   ```

You can pull a image from docker hub like this:

   ```bash
   docker pull docker.mirror.nbtca.space/library/alpine:latest
   ```
