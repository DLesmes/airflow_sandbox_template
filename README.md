# Airflow Sandbox Template
Airflow basic and general functionalities to get started on airflow

# General documentation

[https://airflow.apache.org/docs/](https://airflow.apache.org/docs/)

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












