# Mukti 2017 official website


## Built on top of: Fest Management System

[![Join the chat at https://gitter.im/NIT-dgp/General](https://badges.gitter.im/gitterHQ/gitterHQ.github.io.svg)](https://gitter.im/NIT-dgp/General)

[NIT-dgp/festcms](https://github.com/NIT-dgp/festcms/)

## Prerequisites

### Database

Install sqlite3 for development

* Mac OS X: Mac ships with sqlite3 already installed
* Ubuntu/Debian: `sudo apt-get install sqlite3`
* Fedora/Red Hat/CentOS: `sudo yum install sqlite`

### python-pip

Install pip for python3

* Mac OS (via easy_install): `sudo easy_install pip` 
* Debian/Ubuntu: `sudo apt-get install python3-pip`
* Fedora/CentOS: `sudo yum install python-pip python-wheel`

## Deployment

1. Clone the repository with `git clone git@github.com:ghoshbishakh/festcms.git`
2. Enter the directory using `cd festcms`
3. Copy `festcms/settings.py.example` to `festcms/settings.py`
4. Enter any arbitary key in the `SECRET_KEY` field in `settings.py`
5. To setup mail server, enter the details in email testing section of `settings.py`
6. Ensure that you have python3 set as default. You can do this by `alias python=python3`
7. Run `pip install -r requirements.txt` to install all dependencies
8. Run migrations using `python manage.py migrate`
9. Run server with `python manage.py runserver`
10. Ok you are all set! Visit http://localhost:8000 in your browser
