# Lab 4 - Django and Flask
I pledge my honor that I have abided by the Stevens Honor System.

# Labs 4A and 4B: Django and Django REST

### pip3 -V

```
pi@raspberrypi:~/CPE-322 $ pip3 -V
pip 20.3.4 from /usr/lib/python3/dist-packages/pip (python 3.9)
```

### pip3 list

```
pi@raspberrypi:~/CPE-322 $ pip3 list
Package           Version
----------------- ---------
arandr            0.1.10
astral            2.2
astroid           2.5.1
asttokens         2.0.4
automationhat     0.2.0
beautifulsoup4    4.9.3
blinker           1.4
blinkt            0.1.2
buttonshim        0.0.2
Cap1xxx           0.1.3
certifi           2020.6.20
chardet           4.0.0
click             7.1.2
colorama          0.4.4
colorzero         1.1
cryptography      3.3.2
cupshelpers       1.0
dbus-python       1.2.16
distro            1.5.0
docutils          0.16
drumhat           0.1.0
envirophat        1.0.0
ExplorerHAT       0.4.2
Flask             1.1.2
fourletterphat    0.1.0
geographiclib     1.52
geopy             2.2.0
gpiozero          1.6.2
html5lib          1.1
idna              2.10
isort             5.6.4
itsdangerous      1.1.0
jdcal             1.4.1
jedi              0.18.0
Jinja2            2.11.3
lazy-object-proxy 0.0.0
logilab-common    1.8.1
lxml              4.6.3
MarkupSafe        1.1.1
mccabe            0.6.1
microdotphat      0.2.1
mote              0.0.4
motephat          0.0.3
mypy              0.812
mypy-extensions   0.4.3
numpy             1.19.5
oauthlib          3.1.0
olefile           0.46
pantilthat        0.0.7
parso             0.8.1
pexpect           4.8.0
pgzero            1.2
phatbeat          0.1.1
pianohat          0.1.0
picamera          1.13
piglow            1.2.5
pigpio            1.78
Pillow            8.1.2
pip               20.3.4
psutil            5.8.0
pycairo           1.16.2
pycups            2.0.1
pygame            1.9.6
Pygments          2.7.1
PyGObject         3.38.0
pyinotify         0.9.6
PyJWT             1.7.1
pylint            2.7.2
pyOpenSSL         20.0.1
pyserial          3.5b0
pysmbc            1.0.23
python-apt        2.2.1
pytz              2021.3
rainbowhat        0.1.0
reportlab         3.5.59
requests          2.25.1
requests-oauthlib 1.0.0
responses         0.12.1
roman             2.0.0
RPi.GPIO          0.7.0
RTIMULib          7.2.1
scrollphat        0.0.7
scrollphathd      1.2.1
Send2Trash        1.6.0b1
sense-hat         2.2.0
setuptools        52.0.0
simplejson        3.17.2
six               1.16.0
skywriter         0.0.7
sn3218            1.2.7
soupsieve         2.2.1
spidev            3.5
ssh-import-id     5.10
thonny            3.3.14
toml              0.10.1
touchphat         0.0.1
twython           3.8.2
typed-ast         1.4.2
typing-extensions 3.7.4.3
unicornhathd      0.0.4
urllib3           1.26.5
webencodings      0.5.1
Werkzeug          1.0.1
wheel             0.34.2
wrapt             1.12.1
```

### sudo pip3 install

```
pi@raspberrypi:~/CPE-322 $ sudo pip3 install -U setuptools
Looking in indexes: https://pypi.org/simple, https://www.piwheels.org/simple
Requirement already satisfied: setuptools in /usr/lib/python3/dist-packages (52.0.0)
Collecting setuptools
  Downloading https://www.piwheels.org/simple/setuptools/setuptools-60.9.3-py3-none-any.whl (1.1 MB)
     |████████████████████████████████| 1.1 MB 363 kB/s 
Installing collected packages: setuptools
  Attempting uninstall: setuptools
    Found existing installation: setuptools 52.0.0
    Not uninstalling setuptools at /usr/lib/python3/dist-packages, outside environment /usr
    Can't uninstall 'setuptools'. No files were found to uninstall.
Successfully installed setuptools-60.9.3
pi@raspberrypi:~/CPE-322 $ sudo pip3 install -U django
Looking in indexes: https://pypi.org/simple, https://www.piwheels.org/simple
Collecting django
  Downloading https://www.piwheels.org/simple/django/Django-4.0.2-py3-none-any.whl (8.0 MB)
     |████████████████████████████████| 8.0 MB 169 kB/s 
Collecting asgiref<4,>=3.4.1
  Downloading https://www.piwheels.org/simple/asgiref/asgiref-3.5.0-py3-none-any.whl (22 kB)
Collecting sqlparse>=0.2.2
  Downloading https://www.piwheels.org/simple/sqlparse/sqlparse-0.4.2-py3-none-any.whl (40 kB)
     |████████████████████████████████| 40 kB 9.8 kB/s 
Installing collected packages: sqlparse, asgiref, django
Successfully installed asgiref-3.5.0 django-4.0.2 sqlparse-0.4.2
pi@raspberrypi:~/CPE-322 $ sudo pip3 install -U djangorestframework
Looking in indexes: https://pypi.org/simple, https://www.piwheels.org/simple
Collecting djangorestframework
  Downloading https://www.piwheels.org/simple/djangorestframework/djangorestframework-3.13.1-py3-none-any.whl (958 kB)
     |████████████████████████████████| 958 kB 351 kB/s 
Collecting pytz
  Downloading https://www.piwheels.org/simple/pytz/pytz-2021.3-py3-none-any.whl (511 kB)
     |████████████████████████████████| 511 kB 348 kB/s 
Requirement already satisfied: django>=2.2 in /usr/local/lib/python3.9/dist-packages (from djangorestframework) (4.0.2)
Requirement already satisfied: asgiref<4,>=3.4.1 in /usr/local/lib/python3.9/dist-packages (from django>=2.2->djangorestframework) (3.5.0)
Requirement already satisfied: sqlparse>=0.2.2 in /usr/local/lib/python3.9/dist-packages (from django>=2.2->djangorestframework) (0.4.2)
Installing collected packages: pytz, djangorestframework
Successfully installed djangorestframework-3.13.1 pytz-2021.3
pi@raspberrypi:~/CPE-322 $ sudo pip3 install -U django-filter
Looking in indexes: https://pypi.org/simple, https://www.piwheels.org/simple
Collecting django-filter
  Downloading https://www.piwheels.org/simple/django-filter/django_filter-21.1-py3-none-any.whl (81 kB)
     |████████████████████████████████| 81 kB 370 kB/s 
Requirement already satisfied: Django>=2.2 in /usr/local/lib/python3.9/dist-packages (from django-filter) (4.0.2)
Requirement already satisfied: sqlparse>=0.2.2 in /usr/local/lib/python3.9/dist-packages (from Django>=2.2->django-filter) (0.4.2)
Requirement already satisfied: asgiref<4,>=3.4.1 in /usr/local/lib/python3.9/dist-packages (from Django>=2.2->django-filter) (3.5.0)
Installing collected packages: django-filter
Successfully installed django-filter-21.1
pi@raspberrypi:~/CPE-322 $ sudo pip3 install -U markdown
Looking in indexes: https://pypi.org/simple, https://www.piwheels.org/simple
Collecting markdown
  Downloading https://www.piwheels.org/simple/markdown/Markdown-3.3.6-py3-none-any.whl (97 kB)
     |████████████████████████████████| 97 kB 405 kB/s 
Collecting importlib-metadata>=4.4
  Downloading https://www.piwheels.org/simple/importlib-metadata/importlib_metadata-4.11.2-py3-none-any.whl (17 kB)
Collecting zipp>=0.5
  Downloading https://www.piwheels.org/simple/zipp/zipp-3.7.0-py3-none-any.whl (5.3 kB)
Installing collected packages: zipp, importlib-metadata, markdown
Successfully installed importlib-metadata-4.11.2 markdown-3.3.6 zipp-3.7.0
pi@raspberrypi:~/CPE-322 $ sudo pip3 install -U requests
Looking in indexes: https://pypi.org/simple, https://www.piwheels.org/simple
Requirement already satisfied: requests in /usr/lib/python3/dist-packages (2.25.1)
Collecting requests
  Downloading https://www.piwheels.org/simple/requests/requests-2.27.1-py2.py3-none-any.whl (63 kB)
     |████████████████████████████████| 63 kB 203 kB/s 
Requirement already satisfied: urllib3<1.27,>=1.21.1 in /usr/lib/python3/dist-packages (from requests) (1.26.5)
Requirement already satisfied: certifi>=2017.4.17 in /usr/lib/python3/dist-packages (from requests) (2020.6.20)
Requirement already satisfied: idna<4,>=2.5 in /usr/lib/python3/dist-packages (from requests) (2.10)
Collecting charset-normalizer~=2.0.0
  Downloading https://www.piwheels.org/simple/charset-normalizer/charset_normalizer-2.0.12-py3-none-any.whl (44 kB)
     |████████████████████████████████| 44 kB 287 kB/s 
Installing collected packages: charset-normalizer, requests
  Attempting uninstall: requests
    Found existing installation: requests 2.25.1
    Not uninstalling requests at /usr/lib/python3/dist-packages, outside environment /usr
    Can't uninstall 'requests'. No files were found to uninstall.
Successfully installed charset-normalizer-2.0.12 requests-2.27.1
```

### Install MariaDB Server

```
pi@raspberrypi:~ $ sudo apt update
Hit:1 http://raspbian.raspberrypi.org/raspbian bullseye InRelease
Hit:2 http://archive.raspberrypi.org/debian bullseye InRelease
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
24 packages can be upgraded. Run 'apt list --upgradable' to see them.
pi@raspberrypi:~ $ sudo apt install mariadb-server mariadb-client
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
mariadb-client is already the newest version (1:10.5.12-0+deb11u1).
mariadb-server is already the newest version (1:10.5.12-0+deb11u1).
The following package was automatically installed and is no longer required:
  libfuse2
Use 'sudo apt autoremove' to remove it.
0 upgraded, 0 newly installed, 0 to remove and 24 not upgraded.
pi@raspberrypi:~ $ sudo apt install python3-mysqldb
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
python3-mysqldb is already the newest version (1.4.4-2+b1).
The following package was automatically installed and is no longer required:
  libfuse2
Use 'sudo apt autoremove' to remove it.
0 upgraded, 0 newly installed, 0 to remove and 24 not upgraded.
pi@raspberrypi:~ $ sudo pip3 install -U mysqlclient
Looking in indexes: https://pypi.org/simple, https://www.piwheels.org/simple
Requirement already satisfied: mysqlclient in /usr/local/lib/python3.9/dist-packages (2.1.0)
Collecting mysqlclient
  Using cached https://www.piwheels.org/simple/mysqlclient/mysqlclient-2.1.0-cp39-cp39-linux_armv7l.whl (106 kB)
  Downloading https://www.piwheels.org/simple/mysqlclient/mysqlclient-2.0.3-cp39-cp39-linux_armv7l.whl (106 kB)
     |████████████████████████████████| 106 kB 373 kB/s 
pi@raspberrypi:~ $ sudo mysql_secure_installation

NOTE: RUNNING ALL PARTS OF THIS SCRIPT IS RECOMMENDED FOR ALL MariaDB
      SERVERS IN PRODUCTION USE!  PLEASE READ EACH STEP CAREFULLY!

REDACTED

Cleaning up...

All done!  If you've completed all of the above steps, your MariaDB
installation should now be secure.

Thanks for using MariaDB!
```

### Start a Django project

```
pi@raspberrypi:~ $ django-admin startproject stevens
pi@raspberrypi:~ $ cd stevens
pi@raspberrypi:~/stevens $ ls
manage.py  stevens
```

### Start a Django app

```
pi@raspberrypi:~/stevens $ python3 manage.py startapp myapp
pi@raspberrypi:~/stevens $ ls
manage.py  myapp  stevens
```

### Create MySQL database

```
pi@raspberrypi:~/stevens $ sudo mysql -u root -p
Enter password: 
Welcome to the MariaDB monitor.  Commands end with ; or \g.
Your MariaDB connection id is 36
Server version: 10.5.12-MariaDB-0+deb11u1 Raspbian 11

Copyright (c) 2000, 2018, Oracle, MariaDB Corporation Ab and others.

Type 'help;' or '\h' for help. Type '\c' to clear the current input statement.

MariaDB [(none)]> use mysql
Reading table information for completion of table and column names
You can turn off this feature to get a quicker startup with -A

Database changed
MariaDB [mysql]> select user, host from mysql.user;
+-------------+-----------+
| User        | Host      |
+-------------+-----------+
| mariadb.sys | localhost |
| mysql       | localhost |
| root        | localhost |
+-------------+-----------+
3 rows in set (0.007 sec)

MariaDB [mysql]> create user pi@localhost identified by 'PASSWORD';
Query OK, 0 rows affected (0.022 sec)

MariaDB [mysql]> show databases;
+--------------------+
| Database           |
+--------------------+
| information_schema |
| mysql              |
| performance_schema |
+--------------------+
3 rows in set (0.002 sec)

MariaDB [mysql]> show databases;
+--------------------+
| Database           |
+--------------------+
| information_schema |
| mysql              |
| performance_schema |
+--------------------+
3 rows in set (0.002 sec)

MariaDB [mysql]> create database stevens;
Query OK, 1 row affected (0.001 sec)

MariaDB [mysql]> grant all privileges on stevens.* to pi@localhost;
Query OK, 0 rows affected (0.008 sec)

MariaDB [mysql]> quit
Bye
```

### Edit settings.py in ~/stevens/stevens

```
pi@raspberrypi:~/stevens $ cd stevens
pi@raspberrypi:~/stevens/stevens $ ls
asgi.py  __init__.py  __pycache__  settings.py  urls.py  wsgi.py
pi@raspberrypi:~/stevens/stevens $ nano settings.py
```

### Copy urls.py to ~/stevens/stevens

```
pi@raspberrypi:~/stevens/stevens $ cp ~/iot/lesson4/stevens/urls.py .
pi@raspberrypi:~/stevens/stevens $ cd ..
```

### Copy admin.py, models.py, and views.py to ~/stevens/myapp

```
pi@raspberrypi:~/stevens $ cd myapp
pi@raspberrypi:~/stevens/myapp $ ls
admin.py  apps.py  __init__.py  migrations  models.py  tests.py  views.py
pi@raspberrypi:~/stevens/myapp $ cp ~/iot/lesson4/stevens/admin.py .
pi@raspberrypi:~/stevens/myapp $ cp ~/iot/lesson4/stevens/models.py .
pi@raspberrypi:~/stevens/myapp $ cp ~/iot/lesson4/stevens/views.py .
```

### Edit index.html to add the Google Maps API key

```
pi@raspberrypi:~/stevens/myapp/templates/myapp $ cp ~/iot/lesson4/stevens/index.html
</style>
  <script src="https://maps.googleapis.com/maps/api/js?key=REDACTED"></script>
<script>
```

### Copy static files

```
pi@raspberrypi:~/stevens/myapp/templates/myapp $ cd ~/stevens/myapp/static
pi@raspberrypi:~/stevens/myapp/static $ cp ~/iot/lesson4/static/favicon.ico .
pi@raspberrypi:~/stevens/myapp/static $ mkdir myapp
pi@raspberrypi:~/stevens/myapp/static $ cd myapp
pi@raspberrypi:~/stevens/myapp/static/myapp $ cp ~/iot/lesson4/static/*css .
pi@raspberrypi:~/stevens/myapp/static/myapp $ cp ~/iot/lesson4/static/*js .
pi@raspberrypi:~/stevens/myapp/static/myapp $ cd ~/stevens
```

### Run Django server (error)

```
pi@raspberrypi:~/stevens $ python3 manage.py makemigrations myapp
Migrations for 'myapp':
  myapp/migrations/0001_initial.py
    - Create model TemperatureData
pi@raspberrypi:~/stevens $ python3 manage.py migrate
Operations to perform:
  Apply all migrations: admin, auth, contenttypes, myapp, sessions
Running migrations:
  Applying contenttypes.0001_initial... OK
  Applying auth.0001_initial... OK
  Applying admin.0001_initial... OK
  Applying admin.0002_logentry_remove_auto_add... OK
  Applying admin.0003_logentry_add_action_flag_choices... OK
  Applying contenttypes.0002_remove_content_type_name... OK
  Applying auth.0002_alter_permission_name_max_length... OK
  Applying auth.0003_alter_user_email_max_length... OK
  Applying auth.0004_alter_user_username_opts... OK
  Applying auth.0005_alter_user_last_login_null... OK
  Applying auth.0006_require_contenttypes_0002... OK
  Applying auth.0007_alter_validators_add_error_messages... OK
  Applying auth.0008_alter_user_username_max_length... OK
  Applying auth.0009_alter_user_last_name_max_length... OK
  Applying auth.0010_alter_group_name_max_length... OK
  Applying auth.0011_update_proxy_permissions... OK
  Applying auth.0012_alter_user_first_name_max_length... OK
  Applying myapp.0001_initial... OK
  Applying sessions.0001_initial... OK
pi@raspberrypi:~/stevens $ python3 manage.py createsuperuser
Username (leave blank to use 'pi'): 
Email address: twang51@stevens.edu
Password: 
Password (again): 
Superuser created successfully.
pi@raspberrypi:~/stevens $ pi@raspberrypi:~/stevens $ python3 manage.py runserver
bash: pi@raspberrypi:~/stevens: No such file or directory
```
