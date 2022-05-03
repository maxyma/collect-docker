run:
	docker run --rm --net=bridge -p 127.0.0.1:8080:80 -v ~/code:/data -d storkmax/nginx-phpfpm7

cli:
	docker run --rm --net=bridge -p 127.0.0.1:8080:80 -v ~/code:/data -it storkmax/nginx-phpfpm7 bash

build:
	docker build -t storkmax/nginx-phpfpm7 .

push:
	docker push storkmax/nginx-phpfpm7

