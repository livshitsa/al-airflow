docker build . -t al-airflow

docker run -d -p 8080:8080 --rm \
   --volume $PWD/dags:/app/airflow/dags \
   --name airflow_container \
   al-airflow