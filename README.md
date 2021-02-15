# Apache Airflow

Default settings to get Apache Airflow Docker up and running

## Initializing the environment

- Clone this repo

- Start databases

```sh
docker-compose up airflow-init
```

- Run Airflow

```sh
docker-compose up
```

- Run CLI

```sh
docker-compose run airflow-worker airflow info
```

## Use Airflow shell script

```sh
chmod +x ./airflow.sh
```

## Create alias
```sh
alias airflow='./airflow.sh
```

## Cleaning up

```sh
docker-compose down --volumes --rmi all
```
