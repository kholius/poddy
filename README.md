# poddy

1. 
dnf install podman podman-compose -y && alias docker="podman"

2.
docker run -it ubuntu bash
docker images 
docker ps -a
docker run -p 80:80 nginx;  docker run -p -d 80:80 nginx

3.
https://podman.io/docs

5.

```bash
echo "That's ma boi!" >> ./nginx-html/index.html && docker run -tid --name nginx docker.io/nginx:1.27 -p 25001:80 -v ./nginx-html:/usr/share/html/ && curl http://localhost:25001 
docker rm nginx -f
```

6.

