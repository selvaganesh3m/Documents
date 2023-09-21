## Restore .sql File into PostgreSQL configured using Docker

**Note**: In docker "5000:80" - 5000 is the port we should open in browser (i.e) localhost:5000

1. Extract the tarball in to folder
    ```bash
    tar -zxvf <file_name>.tar.gz -C /path/to/target/folder
    ```
1. Copy the **`.sql`** to docker
    ```bash
    docker cp ~/path/to/<file_name>.sql <container-name>:/var/lib/postgresql/data/
    ```
1. To go to docker bash (shell)
    ```bash
    docker exec -it <container-name> /bin/bash   
    ```
1. Go to postgres sql shell using below command
    ```bash
    psql -U <username> -d <dbname>
    ```
1. Create Dummay database in POSTGRESQL
    ```bash
    CREATE DATABASE <name-of-your-db>;
    ```
1. Now Quit the postgres shell
    ```bash
    \q
    ```
1. Final Restoration steps:
    ```bash
    psql -U selva -d usa -a -f /var/lib/postgresql/data/usda.sql
    ```
1. Go to psql shell again
1. Check if the DB exists using below query
    ```sql
    SELECT datname FROM pg_database;
    ```
    or
    ```bash
    \l
    ```


