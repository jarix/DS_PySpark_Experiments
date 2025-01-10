# DS_PySpark_Experiments

Some simple Apache Spark Experiments running PySpark Notebooks in local mode (while learning Spark).
Docker files are also included for running the PySpark notebooks against a docker container. 

## Requirements

- Docker and docker-compose installed in the local machine.

## Setup for vanilla PySpark

```
docker-compose up --build
```

Once docker running, point VSCode or Browser to 
```
http://127.0.0.1:8888/lab?token=xyz 
```
Copy and Paste the token (password) from the docker-compose startup spew

## Setup for PySpark with Delta Lake

```
docker-compose -f ./docker-compose-delta.yml up --build
```

Once docker running, point VSCode or Browser to 
```
http://127.0.0.1:8888/ 
```

No password needed for this docker

## Setup for PySpark with MLFlow

```
docker-compose -f ./docker-compose-mlflow.yml up --build
```

Once docker running, point VSCode or Browser to 
```
http://127.0.0.1:8888/ 
```

No password needed for this docker

To access MFlow UI, issue the following command inside docker
```
mlflow ui --host 0.0.0.0
```

Access the MLFlow UI at 
```
http://127.0.0.1:5000/ 
```

## Troubleshooting

Spark UI is available at
```
http://127.0.0.1:4040/ 
```
