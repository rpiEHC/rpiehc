# RPI Embedded Hardware Club Public Website


[Embedded Hardware Club](http://rpiEHC.org)
Rensselaer Polytechnic Institute
Troy, NY, USA

We're a group of students at RPI who share a passion for embedded devices.


## Developer's Guide

Use this guide to quickly start developing for this site. The public website uses [django-cms](https://django-cms.org/). Develop locally using virtualenv, which is in repos for your preferred operating system as `virtualenv` or `virtualenv2`.

### Setting Up the Development Environment

```
$ virtualenv <arbitrary> --distribute
$ cd <arbitrary>
$ source bin/activate
$ git clone https://github.com/rpiEHC/rpiehc.git
$ cd rpiehc
$ pip install -r requirements.txt
$ python manage.py syncdb --all  # skip the --all after first use
$ python manage.py migrate --fake  # skipp the --fake after first use
```

Exit the virtualenv at any time with `deactivate`.

### Running the Development Server

```
$ python manage.py runserver
```
