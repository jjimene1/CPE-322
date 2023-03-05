# Lab 4 - Django and Flask

## Lesson 4 Notes

Django and Flask are both open-source Python based devlepooment frameworks designed to ease code complexity for programmers. While Django is a full stack framework, Flaks is a lightweight microframework but it is also extensible. These can be used to create quick and fast web based projects.

## Lab 4 Implementation

Installation instructions can be found in [the Lesson 4 GitHub](https://github.com/kevinwlu/iot/tree/master/lesson4). The implmentation of the lab was done on a Raspberry Pi 4.

### Django Project "Stevens"

The following are the commands and outputs of running the project "Stevens":

#### Start a Django Project

```bash
jj@raspberrypi:~ $ django-admin startproject stevens
jj@raspberrypi:~ $ cd stevens
jj@raspberrypi:~/stevens $ ls
manage.py  stevens
```

#### Start a Django App

```bash
jj@raspberrypi:~/stevens $ python3 manage.py startapp myapp
jj@raspberrypi:~/stevens $ ls
manage.py  myapp  stevens
```

#### Create MySQL Database

```bash
jj@raspberrypi:~ $ sudo mysql -u root -p
Enter password: -------
MariaDB [(none)]> use mysql
MariaDB [mysql]> select user, host from mysql.user;
MariaDB [mysql]> create user jj@localhost identified by '-------';
MariaDB [mysql]> show databases;
MariaDB [mysql]> create database stevens;
MariaDB [mysql]> grant all privileges on stevens.* to jj@localhost;
MariaDB [mysql]> quit
```

#### Edit settings.py in ~/stevens/stevens

* Follow the [template](https://github.com/kevinwlu/iot/blob/master/lesson4/stevens/settings.txt) from ~/iot/lesson4/stevens/settings.txt, e.g., add an asterisk to ALLOWED_HOSTS and 'myapp' to INSTALLED_APPS.
* The comma after 'myapp' is required.
* ------ changed from MySQL user jj.
* Data was also added from databases which was missing from the settings.py file.

```bash

jj@raspberrypi:~/stevens $ cd stevens
jj@raspberrypi:~/stevens/stevens $ ls
asgi.py  __init__.py  __pycache__  settings.py  urls.py  wsgi.py
jj@raspberrypi:~/stevens/stevens $ emacs settings.py
```

#### Copy urls.py to ~/stevens/stevens

```bash
jj@raspberrypi:~/stevens/stevens $ cp ~/iot/lesson4/stevens/urls.py .
jj@raspberrypi:~/stevens/stevens $ cd ..
```

#### Copy admin.py, models.py, and views.py to ~/stevens/myapp

```bash
jj@raspberrypi:~/stevens $ cd myapp
jj@raspberrypi:~/stevens/myapp $ ls
admin.py  apps.py  __init__.py  migrations  models.py  tests.py  views.py
jj@raspberrypi:~/stevens/myapp $ cp ~/iot/lesson4/stevens/admin.py . 
jj@raspberrypi:~/stevens/myapp $ cp ~/iot/lesson4/stevens/models.py .
jj@raspberrypi:~/stevens/myapp $ cp ~/iot/lesson4/stevens/views.py .
```

#### Copy index.html

```bash
jj@raspberrypi:~/stevens/myapp $ mkdir static templates
jj@raspberrypi:~/stevens/myapp $ cd templates
jj@raspberrypi:~/stevens/myapp/templates $ mkdir myapp
jj@raspberrypi:~/stevens/myapp/templates $ cd myapp
jj@raspberrypi:~/stevens/myapp/templates/myapp $ cp ~/iot/lesson4/stevens/index.html .
```

#### Enabling Google Maps API

*In order to eneable Google Maps API you must create an account at the following [link](https://console.cloud.google.com/welcome?project=midterm-293405). After creating an account you will receive the API key neccessary to get the google maps geolocation working.

#### Copy Static Files

```bash
jj@raspberrypi:~/stevens/myapp/templates/myapp $ cd ~/stevens/myapp/static
jj@raspberrypi:~/stevens/myapp/static $ cp ~/iot/lesson4/static/favicon.ico .
jj@raspberrypi:~/stevens/myapp/static $ mkdir myapp
jj@raspberrypi:~/stevens/myapp/static $ cd myapp
jj@raspberrypi:~/stevens/myapp/static/myapp $ cp ~/iot/lesson4/static/*css .
jj@raspberrypi:~/stevens/myapp/static/myapp $ cp ~/iot/lesson4/static/*js .
jj@raspberrypi:~/stevens/myapp/static/myapp $ cd ~/stevens
```

#### After the first time, skip these three steps if no changes

```bash
jj@raspberrypi:~/stevens $ python3 manage.py makemigrations myapp 
jj@raspberrypi:~/stevens $ python3 manage.py migrate
jj@raspberrypi:~/stevens $ python3 manage.py createsuperuser
Username (leave blank to use 'jj'):
Email address: jjimene6@stevens.edu
Password: ------
Password (again): ------
Superuser created successfully.
```

#### Run the Django Project

```bash
jj@raspberrypi:~/stevens $ python3 manage.py runserver
```

#### Open the Chromium browser on Raspberry Pi via VNC Viewer

Go to <http://127.0.0.1:8000/admin>

Login with Django administration username (jj) and password.

Click temperature data to add:

* Date and time in YYYY-MM-DD HH:MM:SS.
* Temperature in Fahrenheit
* Latitude 40.7451
* Longitude -74.0255

Click SAVE.

View app at <http://127.0.0.1:8000>.

#### Working app and Output Website

If everything went succesfully the admin site should look like this:

![Working Admin Site](DjangoAdmin.png)

The website should look like this after adding the appropiate data:

![Working Website](Website.png)
