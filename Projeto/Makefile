#Remover imagens
delete:
	docker rmi projetoconsumer
	docker rmi projetoproducer

#Remover volumes
remove:
	sudo rm -r minio
	sudo rm -r rabbitmq
	sudo rm -r redis

#Remover os containers e volumes
reset:
	docker-compose down
	docker rmi projetoconsumer
	docker rmi projetoproducer
	sudo rm -r minio
	sudo rm -r rabbitmq
	sudo rm -r redis

up:
	docker-compose up --build

network:
	docker network ls



