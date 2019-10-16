# recipe-api
Recipe REST API with Python, Django &amp; Docker using test driven development (TDD)
## Docker
1. Add the **Dockerfile** all the dependecies that you need in the project
    * Requirements.txt 

2. Build the project `docker build .`
### Configuration docker
1. Add the file **docker-compose.yml** 
2. `docker-compose build` (which build our image using the docker-compose configuration)
2. `docker-compose run app sh -c "django -admin.py startproject app."`

