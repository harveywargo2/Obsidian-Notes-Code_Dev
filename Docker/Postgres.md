# Reference
- https://www.docker.com/blog/how-to-use-the-postgres-docker-official-image/
- https://hub.docker.com/_/postgrese

# Commands 
Pull Docker Image
```
docker pull postgress
```


```
docker run --name <dbname> -p 5432:5432 -e POSTGRES_PASSWORD=mysecretpassword -d postgres
```

Spin Up Docker Container with attached volume 
```
docker run --name postgres-detecto -e POSTGRES_PASSWORD=detecto -p 5432:5432 -v postgres-detecto:/var/lib/postgressql/data -d postgres
```