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

```bash
podman build -f Dockerfile -t nginx-joke
```
l'index.html est directement definit dans l'image donc pas besoin de post configuration

7.


8.


```bash
docker-compose up -d
```
Passer sous docker compose permet, à partir d'un fichier, definir l'ensemble des conteneurs avec leurs dependances, storage, env vars et intéractions.
On configure la base Mysql par des variable d'environnement.



