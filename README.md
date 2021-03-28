# Spark an Jupyter notebooks on docker

 Run Apache spark and jupyter notebooks using docker.

## Run container and pass your volume to mount:
```sh
docker run -it --rm -p 8888:8888 -p 4040-4050:4040-4050 -v <your_volume>:/home/jovyan/work jupyter/pyspark-notebook
```

### Eg. mounted volume <your_volume>:

`/Users/<your_user>/Desktop/spark-on-docker/home:/home/jovyan/work`