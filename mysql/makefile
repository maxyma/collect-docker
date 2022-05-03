run:
	docker run --rm -p 127.0.0.1:3306:3306 \
	-v $(PWD)/data:/var/lib/mysql \
	-e MYSQL_ROOT_PASSWORD="dh123" \
	-e TZ=Asia/Shanghai -e MYSQL_INITDB_SKIP_TZINFO \
	-d mariadb:10.3 \
	--character-set-server=utf8mb4 --collation-server=utf8mb4_unicode_ci 

