# 02_web_server_app
1. Make docker image
```
$ docker build -t app_test ./
```

2. Run docker container

```
$ docker run -p 3000:3000 -d app_test
```

3. Check

```
$ curl http://localhost:3000
```
 
4. Delete docker container
```
$ docker ps
$ docker stop <<container id>>
$ docker rm <<container id>>
```

5. Delete docker image
```
$ docker rmi app_test
```
