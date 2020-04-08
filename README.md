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

Run the test

* `docker-compose run --rm app sh -c "python manage.py test && flake8"`

Add migrations (new models)
* `docker-compose run --rm app sh -c "python manage.py makemigrations core"`

If not opening in browser
`docker-machine ip default` - it shows the ip for opening with port 8000