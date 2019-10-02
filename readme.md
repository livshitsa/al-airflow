docker build . -t al-airflow

in bash shell:

docker run -d -p 8080:8080 --rm \
   --volume $PWD/dags:/app/airflow/dags \
   --name airflow_container \
   al-airflow
   
in powershell on wondows:

docker run -d -p 8080:8080 --rm `
   --volume ${PWD}/dags:/app/airflow/dags `
   --name airflow_container al-airflow
