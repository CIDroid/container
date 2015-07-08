# Nginx Proxy

- Pull this repo: [nginx-proxy](https://github.com/jwilder/nginx-proxy)
- Replace nginx.tmpl


## Run image

```
docker run -d -p 80:80 --privileged=true -v /var/run/docker.sock:/tmp/docker.sock:ro -v /home/ubuntu/work:/work nginx-proxy
```