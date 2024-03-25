start:
	$(info Run!)
	podman-compose -f docker-compose.yaml up -d --remove-orphans

stop:
	$(info stopping VC)
	podman-compose -f docker-compose.yaml rm -s -f

restart: stop start

clean: stop
	podman volume rm datastore_mongo_data_demo
