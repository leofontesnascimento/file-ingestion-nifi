build:
	docker-compose build

build-no-cache:
	docker-compose build --no-cache

pull:
	docker-compose pull

start:
	docker volume create --name=nifi_conf
	docker volume create --name=nifi_database_repository
	docker volume create --name=nifi_flowfile_repository
	docker volume create --name=nifi_content_repository
	docker volume create --name=nifi_provenance_repository
	docker volume create --name=nifi_state
	docker volume create --name=nifi_logs
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