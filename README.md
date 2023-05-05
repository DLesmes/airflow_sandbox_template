# Airflow Sandbox Template
Airflow basic and general functionalities to get started on airflow

# General documentation

[https://airflow.apache.org/docs/](https://airflow.apache.org/docs/)

## Instalation

### Cloning this repo

You can use this repo to build you own airflow application just follow the next steps:

```
git clone git@github.com:DLesmes/airflow_sandbox_template.git
```
```
cd airflow_sandbox_template
```
```
curl -LfO 'https://airflow.apache.org/docs/apache-airflow/2.5.3/docker-compose.yaml'
```
There is a more recent [version 2.6.0](https://airflow.apache.org/docs/apache-airflow/stable/howto/docker-compose/index.html#fetching-docker-compose-yaml)

* If you do not want to see the example DAG's, you can set this tag as false, it is on line 65 of the docker-compose.yaml file

      AIRFLOW__CORE__LOAD_EXAMPLES: 'false'

Start Docker, you must to have it installed previously
```
docker compose up
```
### From scratch

Just follow the next steps on your local console:

```
mkdir my_airflow_project
cd my_airflow_project
mkdir -p ./dags ./logs ./plugins ./scripts
echo -e "AIRFLOW_UID=$(id -u)" > .env
```
```
curl -LfO 'https://airflow.apache.org/docs/apache-airflow/2.5.3/docker-compose.yaml'
```
There is a more recent [version 2.6.0](https://airflow.apache.org/docs/apache-airflow/stable/howto/docker-compose/index.html#fetching-docker-compose-yaml)

* If you do not want to see the example DAG's, you can set this tag as false, it is on line 65 of the docker-compose.yaml file

      AIRFLOW__CORE__LOAD_EXAMPLES: 'false'

Start Docker, you must to have it instaled previously
```
docker compose up
```

## General Folder Distribution / Three

```
airflow/
│
├── dags/
│   ├── example_dag.py
│   └── ...
│
├── plugins/
│   ├── my_plugin.py
│   └── ...
│
├── config/
│   ├── airflow.cfg
│   └── ...
│
├── logs/
│   ├── dag_processing.log
│   ├── scheduler.log
│   └── ...
│
├── scripts/
│   ├── airflow
│   ├── airflow.cfg
│   └── ...
│
├── tests/
│   ├── test_example_dag.py
│   ├── test_my_plugin.py
│   └── ...
│
└── README.md
```

In this diagram, the main airflow/ directory contains several subdirectories, including 
* dags/ which holds the DAG definition files, 
* plugins/ which holds any custom plugins used in the DAGs, 
* config/ which holds the Airflow configuration files, 
* logs/ which holds the Airflow logs, 
* scripts/ which holds the Airflow command line scripts, 
* tests/ which holds the test files for the DAGs and plugins, and 
* README.md which contains the repository's documentation.












