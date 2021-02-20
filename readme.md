# Learning Log 

## How to setup the project

1. Create a virtual environment, name it as  `ll_env`

2. From `terminal` in `Pycharm IDE` run:
    ```bash
    pip install -r requirements.txt
    ```

3. Run the built-in webserver provided by Django framework by running the below command in `terminal`

    ```bash
    python manage.py runserver
    ```    
4. If all is good, webserver would start and serve our site here - <http://127.0.0.1:8000/>

5. Verify all are working correctly
    * Chess <http://127.0.0.1:8000/topics/1/>
    * Rock climbing - <http://127.0.0.1:8000/topics/2/>
    
## update requirements.txt with all latest dependencies

* Always after installing any packages in the virtual environment `ll_env`.
* Run the command in terminal

    ```bash
    pip freeze > requirements.txt
    ```
## Commands used in this project - to be updated

1. pip install django
2. django-admin startproject learning_log .
    3. python manage.py migrate
    4. python manage.py runserver
5. python manage.py makemigrations learning_logs
6. python manage.py createsuper user
    username : ll_admin 
    password : Password
7. python manage.py shell
    from learning_logs.models import Topic
    Topic.objects.all()
8. python manage.py startapp users
    created a user with below
    username : swarna
    password : admin@123
    
    New profile
    Username : swarna@test1
    Password : admin@123
   
9. pip install django-bootstrap4    
10. https://getbootstrap.com/   

11. Installing Heroku
    1. https://signup.heroku.com/account - Signup
    2. https://dashboard.heroku.com/apps
    3. Run below command in active server terminal
        pip install psycopg2==2.7.*
        pip install django-heroku
        pip install gunicorn
    4. Make a requirementss.txt (as we already have a requirements.txt)
    5. Get the version of python for heroku
        python --version
    6. git config --global user.name "username"
    7. git config --global user.email "email"
    
Below are steps to be followed to add to git
    1. Use same termina
        git init
        git add .
        git commit -am "Ready for deployment to heroku"

we dont push all local data to heroku so create a new super user
    username : ll_admin 
    password : admin@123
        


    

  
