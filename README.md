# Containers para uso general del PHP

## Uso


### Crear la imagen ejecutar 

```bash

./build.sh

```

o el directamente el comando docker que sigue

```bash

docker build --force-rm=true --no-cache=true . -t imit/mean

```
	

### Crear container

```bash

./run.sh

```

o directamente el comando docker que sigue

```bash

sudo docker run -d --shm-size=1g  -i -t -p 127.0.0.1:33000:3000 -p 127.0.0.1:34200:4200 -p 127.0.0.1:30080:80 -p 127.0.0.1:30443:443 -p 127.0.0.1:35279:35279 -p 127.0.0.1:38080:8080 -h dc-mean  -v /Users/luiz.quelves/projects/work/apps/app-demo:/opt/app -P --name="dc-mean" imit/mean 


```








