run:
	docker run --rm -d -p 127.0.0.1:2222:22 \
		-v /var/run/docker.sock:/var/run/docker.sock \
		storkmax/developer

build:
	docker build -t storkmax/developer .

push:
	docker push storkmax/developer

