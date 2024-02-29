

run:
	docker pull emqx/emqx
	docker run -d --name emqx -p 1883:1883 -p 8081:8081 -p 18083:18083 emqx/emqx

stop:
	docker stop emqx
	docker rm emqx

clean: stop
	docker rmi emqx/emqx
