# 01_web_server_apache
1. Make docker image
```
$ docker build -t apache_test ./
```

2. Run docker container

```
$ docker run -p 8000:80 -d apache_test
```

3. Check

```
$ curl http://localhost:8000
```
 
4. Delete docker container
```
$ docker ps
$ docker stop <<container id>>
$ docker rm <<container id>>
```

5. Delete docker image
```
$ docker rmi apache_test
```
