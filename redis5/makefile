run:
	docker run --rm --net=bridge -p 127.0.0.1:6379:6379 -v $(PWD):/data -d storkmax/redis5 redis-server /data/redis.conf

build:
	docker build -t storkmax/redis5 .

push:
	docker push storkmax/redis5


