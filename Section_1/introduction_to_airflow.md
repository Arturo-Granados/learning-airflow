# learning-airflow
<a><img src="./images/apache_airflow.webp"/></a>
Overall, Apache Airflow is a powerful tool for data engineering that empowers users to create, manage, and scale complex data pipelines with ease and confidence. Its active community, growing ecosystem, and flexible design make it a popular choice for data-driven organizations of all sizes and domains.

## What is Apache Airflow

Apache Airflow is an open-source platform to programmatically author, schedule, and monitor workflows or data pipelines.

## Why Airflow?

Airflow is a batch workflow orchestration platform. The Airflow framework contains operators to connect with many technologies and is easily extensible to connect with a new technology.

## Components

### Principals 

Web server -> Flask server with Giunicorn that give access to the UI.

Scheduler  -> Schedule the tasks.

Metastore  -> Database where the metadata are store.

### Aditionals

Executor   -> Class definning how your task should be executed. 

Worker     -> Process/sub process executing your tasks.

### Diference between Executor and Worker
The executor define how your taks are going to be  executed in wich system and a worker is the procces where yuor task is effetively executed.

## Important concepts

### Taks
Taks is a basic unit of execution of airflow(task are arranged into dag's).

### DAG'S: 
Directed Acyclic Graph. is a collection of tasks with dependencies that represent a workflow or data pipeline. A DAG is defined as a Python script that creates a DAG object and adds tasks to it using Airflow's Python API.

### Workflow
In Apache Airflow, a workflow refers to a sequence of tasks that are orchestrated to perform a specific data processing or data integration job.

### Operators: 
Is a class that defines a single task in a DAG.

### kind of operators:

Action operator  -> excute something

Tranfer operator -> transform data

Sensor operatos  -> allow you to wait for  a condition to be met before getting complited

## What airflow is not?
Is not a data streaming solution neither a data processing framework.