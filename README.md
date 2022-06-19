## Personal Portfolio with Django

It has:
- create a database, design the layout for your website,
- add and update URL paths. 
- connect your Django projects to Postgres, 
- add static files and URLs, and more.


<img src="" width="800" height="400"  />  

<img src="" width="800" height="400"  />  

<img src="" width="800" height="400"  />  

<img src="" width="800" height="400"  />  

<img src="" width="800" height="400"  />  

<img src="" width="800" height="400"  />  

<img src="" width="800" height="400"  />  

<img src="" width="800" height="400"  />  

<img src="" width="800" height="400"  />  





## commands

1 

pipenv install django

pip install django

~= which will ensure security updates for Django, such as 3.1.1, 3.1.2, and so on.

------------------------------------------------------------------------------

check

django-admin --version

------------------------------------------------------------------------------

activate virtual environment:

pipenv shell

------------------------------------------------------------------------------

if this runs with no error:

2

django-admin startproject portfolio 

#rename the top level of portfolio to portfolio-project

cd portfolio-project




so my virtual environment has Django installed properly.

here without (.) to the command, it will create config folder in config folder

------------------------------------------------------------------------------

3

django-admin startapp pizza


4

pip3 install django-widget-tweaks 



------------------------------------------------------------------------------

running Django’s local web server

python manage.py runserver

exit

------------------------------------------------------------------------------

pipenv shell

exit


------------------------------------------------------------------------------

python manage.py startapp pages

• admin.py is a configuration file for the built-in Django Admin app

• apps.py is a configuration file for the app itself

• migrations/ keeps track of any changes to our models.py file so our database and models.py stay in sync

• models.py is where we define our database models which Django automatically translates into database tables

• tests.py is for our app-specific tests

• views.py is where we handle the request/response logic for our web app

------------------------------------------------------------------------------
Run:

python manage.py runserver

------------------------------------------------------------------------------
test:

python manage.py test

------------------------------------------------------------------------------

apply the migrations:

python manage.py migrate

change the user:

python manage.py createsuperuser

nilecrocodile

mohamed.reda.007007@gmail.com 

12345678

------------------------------------------------------------------------------
after creating new model at notes, lets deal with the database:

python manage.py makemigrations

after showing the migration of which user who created the note, apply the default athe terminal as:

1

1

then apply the migrations:

python manage.py migrate

check:

python manage.py shell

from django.contrib.auth.models import User

user = User.objects.get(pk=1)

user

user.notes.count()

------------------------------------------------------------------------------
