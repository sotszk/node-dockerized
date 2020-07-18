# node-dockerized

nodejs のアプリケーションを docker 環境で実行するサンプルコードです。

## Getting started

```
$ docker build -t <your-name>/node-dockerized .

$ docker run -p 8000:8080 -d --name test <your-name>/node-dockerized

$ docker exec -it test /bin/bash

$ [root@<container id>:usr/src/app#] curl localhost:8080
# -> Hello world!

$ [root@<container id>:usr/src/app#] exit

$ curl localhost:8000
# -> Hello world!

$ docker rm -f test

$ docker ps -ls
# -> nothing running
```
