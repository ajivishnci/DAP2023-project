# Project Setup with Docker and Docker-compose

This project is set up using Docker and Docker-compose. Docker manages the application with `Mongo DB` and `PostgreSQL` databases, along with `JupyterLab`.

## Prerequisites
- Docker needs to be installed on the machine.
- Python should be installed.

# Steps to Run the Project

1. Navigate to the project folder location and open a Windows command prompt.

    ```bash
    cd path/to/project/folder
    ```

2. Execute the `docker` script.

    ```bash
    docker-compose up
    ```

3. Check if the all the container images is up and running, Mongo DB`, `JupyterLab` and `PostgreSQL`

4. Open the `Jupyter notebook` link which you would see in the command line `ctrl + click`
    ```bash
    https://127.0.0.1
    ```
5. Upload the notebooks to Jupyter Lab in the `notebooks` source folder.

6. Run the Python notebooks.

7. Execute the `docker` script when done.

    ```bash
    docker-compose down
    ```

Make sure to follow these steps in sequence to successfully run the project.

### Note:
If you encounter issues with Docker containers for MongoDB or PostgreSQL:
Try restarting the container.

You can try the following commands in the terminal:

```bash
docker restart my_postgresql
docker stop my_postgresql
docker rm my_postgresql
docker volume ls
docker volume rm project_postgresql_data
docker-compose up -d
