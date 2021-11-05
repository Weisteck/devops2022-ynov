```bash
docker build -t tp1 .
# on peut preciser le dockerfile que l on veut lancer avec l argument file
# docker build -t tp1bis -f ./Dockerfile2 .

docker run --name tp1 -v "$(pwd)/data:/usr/share/nginx/html" -p 8000:80 tp1

docker logs tp1

# creer un network
docker network create commun

# add option --network commun
```
