build:
	docker-compose build

build-no-cache:
	docker-compose build --no-cache

pull:
	docker-compose pull

start:
	docker-compose up -d

stop:
	docker-compose down

# make logs SERVICE=service-name
logs:
	docker-compose logs -f --tail 40 ${SERVICE}

# make network-create NETWORK=external-network-name
network-create:
	docker network create ${NETWORK}

# make network-remove NETWORK=external-network-name
network-remove:
	docker network rm ${NETWORK}

# make console SERVICE=service-name
console:
	docker-compose exec ${SERVICE} bash