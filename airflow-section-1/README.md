## Apache AirFLow

### How to Run

1. Run the container (run the below commands while inside this folder):
    ```shell
    make build &&
    ```

2. See if the container is running as expected:
    ```shell
    docker ps
    ```

3. Access the container:
    ```shell
    make run
    ```

4. Run the following commands, one by one, inside the container terminal (option):
    ```shell
    airflow db init
    ```
    ```shell
    airflow scheduler &
    ```
    ```shell
    airflow users  create --role Admin --username admin --email admin --firstname admin --lastname admin --password admin
    ```
    ```shell
    airflow webserver &
    ```

5. Open the browser on [localhost:8080](https://localhost:8080)
    ```shell
    username: admin
    password: admin
    ```
    
## Must Read
    [AirFlow - Package Extras](https://airflow.apache.org/docs/apache-airflow/stable/extra-packages-ref.html)