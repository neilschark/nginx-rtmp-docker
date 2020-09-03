# nginx-rtmp-docker

Based on: https://github.com/tiangolo/nginx-rtmp-docker

I recommend using the docker-compose.yml for deployment.

```
version: '3'
services:
  streaming-nginx:
    image: njay289/nginx-rtmp-docker:latest
    container_name: streaming-nginx
    ports:
      - 0.0.0.0:1935:1935
    restart: unless-stopped
```
