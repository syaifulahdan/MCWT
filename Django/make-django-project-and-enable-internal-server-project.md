### Make django project and enable internal server project

A.  create a project django
project that we will create will we put into the virtual environment python1, do not forget to activate the first directory.

1.Start the terminal and then go to the directory and activate python1
  <pre>
  (python1) bertopeng17@bertopeng17-ThinkPad-T520:~/Desktop/python1$ <b>. bin/activate</b>
  (python1) bertopeng17@bertopeng17-ThinkPad-T520:~/Desktop/python1$
  </pre>
2. The first thing we do is run the command <b>django-admin.py startproject</b> [project name], to create a project, for example:
  <pre>
  (python1) bertopeng17@bertopeng17-ThinkPad-T520:~/Desktop/python1$ <b>django-admin.py startproject telematika</b>
  (python1) bertopeng17@bertopeng17-ThinkPad-T520:~/Desktop/python1$ 
  </pre>

3. To bootstrap the database (this uses SQLite by default) on more recent versions of Django, you can type
   <pre>python manage.py migrate</pre>

    <pre>
    (python1) bertopeng17@bertopeng17-ThinkPad-T520:~/Desktop/python1/telematika$ python manage.py migrate
     Operations to perform:
    Apply all migrations: admin, contenttypes, auth, sessions
    Running migrations:
    Rendering model states... DONE
    Applying contenttypes.0001_initial... OK
    Applying auth.0001_initial... OK
    Applying admin.0001_initial... OK
    Applying admin.0002_logentry_remove_auto_add... OK
    Applying contenttypes.0002_remove_content_type_name... OK
    Applying auth.0002_alter_permission_name_max_length... OK
    Applying auth.0003_alter_user_email_max_length... OK
    Applying auth.0004_alter_user_username_opts... OK
    Applying auth.0005_alter_user_last_login_null... OK
    Applying auth.0006_require_contenttypes_0002... OK
    Applying auth.0007_alter_validators_add_error_messages... OK
    Applying sessions.0001_initial... OK
    </pre>
    [alt img](https://github.com/syaifulahdan/MCWT/blob/master/Django/image/Screenshot%20from%202016-04-17%2015:05:01.png)
    
4. You will be asked to create an administrative user as part of this process. Select a username, email address, and password for the user. If you used the migrate command above, you'll need to create the administrative user manually. You can create an administrative user by typing: 
<pre>python manage.py createsuperuser</pre>
<pre>
(python1) bertopeng17@bertopeng17-ThinkPad-T520:~/Desktop/python1/telematika$ <b>python manage.py createsuperuser</b>
Username (leave blank to use 'bertopeng17'): <b>telematika</b>
Email address: <b>syaifulahdan@gmail.com</b>
Password: <b>**********</b>
Password (again): 
Superuser created successfully.
(python1) bertopeng17@bertopeng17-ThinkPad-T520:~/Desktop/python1/telematika$ 
</pre>

5. 

4. Look in the directory python1 there will be a new project which we add is

  ![alt img] (https://github.com/syaifulahdan/MCWT/blob/master/Django/image/Screenshot%20from%202016-04-16%2015:59:59.png)
  
  ![alt img] (https://github.com/syaifulahdan/MCWT/blob/master/Django/image/Screenshot%20from%202016-04-16%2016:00:27.png)
  
  ![alt img] (https://github.com/syaifulahdan/MCWT/blob/master/Django/image/Screenshot%20from%202016-04-16%2016:00:52.png)

B.  activated the internal server project , project name : <b>telematika</b>

1. go to the directory project we have created is Telematika, Use the <b>python manage.py runserver </b>
