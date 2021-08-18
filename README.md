# Apache Airflow

Default settings to get Apache Airflow Docker up and running

## Initializing the environment

- Clone this repo

- Start databases

```sh
docker-compose up airflow-init -d
```

- Run Airflow

```sh
docker-compose up -d
```

- Run CLI

```sh
docker-compose run airflow-worker airflow info -d
```

## Use Airflow shell script

```sh
chmod +x ./airflow.sh
```

## Create alias
```sh
alias airflow="$(pwd)/airflow.sh"
```

## Cleaning up

```sh
docker-compose down --volumes --rmi all
```
