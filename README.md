# Spark on docker
- Run spark using docker.

## Run docker compose:
```sh
docker-compose up
```

### To run a single container:
```sh
docker start spark-master
docker start spark-worker-1
```

### To Connect to container:
```sh
docker exec -it spark-master bash
docker exec -it spark-worker-1 bash
```

### Mounted Volume:

- ./home => /home

## Run basic example
spark/bin/spark-submit /home/codeExample.py home/data.csv