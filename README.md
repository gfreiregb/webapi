REST API built with DjangoRestFramework and Python  

Commands to run it locally:  
  
git clone https://github.com/gfreiregb/webapi.git  
cd webapi  
python3 -m venv venv  
source venv/bin/activate  
pip install django  
pip install djangorestframework  
brew install postgresql@14  
pip install psycopg2  
brew services start postgresql@14  
psql postgres  
CREATE ROLE youruser LOGIN; -> Update the settings.py file with the user name you created. Line 81 DATABASES  
exit  
cd webapi  
python manage.py migrate  
python3 manage.py runserver  
http://127.0.0.1:8000/users/  
  
Any changes to existing models or the addition of new models require new migrations to be performed before running the server.  
  
More on this:  
https://docs.djangoproject.com/en/4.2/topics/migrations/  
