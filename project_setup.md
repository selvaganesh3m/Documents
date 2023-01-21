## Setting up new Django Project in docker


1. Create new directry (expense-tracker) with project name
1. Open that directory (expense-tracker) in **VS code**
1. In the expense-tracker create file **docker-compose.yml** and fill necessary conents
1. Create **Dockerfile**  as well and name it 
1. Fill necessary contents in Dockerfile
1. Create **requirements.txt** in same directory and fill the requiremets
1. Then type the below command to create project inside docker

    ```bash
        docker-compose run <web-container-name> django-admin start project           <project-name> .
    ```
1. If the above command doesn't work use **sudo** before that
1. Now you've created a project.

