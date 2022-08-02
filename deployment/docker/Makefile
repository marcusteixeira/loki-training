install-plugin:
	docker plugin install grafana/loki-docker-driver:latest --alias loki --grant-all-permissions

all: install-plugin run view-logs 
run:
	docker-compose up -d

view-logs:
	docker-compose logs

stop:
	docker-compose down -v