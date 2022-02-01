**Pizza App API**
Source code for Pizza App

The project uses:  

Python  3.9.  
Django  3.2.6  
Django Rest Framework  3.12.4  
Postgres  13.3   
Flake8  3.9.2

**Getting started**    
To start project, run:    

```
docker-compose up  
```

The API will then be available at http://127.0.0.1:8000 

If you need to make rebuild, you have to use this command:

```
docker-compose build
```

After that repeat the command docker-compose up for launching the project.
   
**Commands:**.  
When you need to use a python manage.py command, you have to write (just an example):       

```
docker-compose run app sh -c "your command"     
docker-compose run app sh -c "python manage.py startapp new_app"
```

You can launch the tests using this command:      

`docker-compose run app sh -c "python manage.py test"`

You can also use flake8 when you want to check the code style of the project:      

`docker-compose run app sh -c "python manage.py test && flake8"`


**Admin part:**
You can enter in the admin part using this url adress:

http://127.0.0.1:8000/admin/

You can create a superuser (admin) using this command (if you don't have it yet):

```
docker-compose run app sh -c "python manage.py createsuperuser"
```


