# BanTech:

> **MVP** - Final project for Holberton School Foundations program.

All your bank information in one place.

![enter image description here](https://github.com/JuanManuelReyes/bantech-mvp/blob/main/flask_server/src/static/img/a.png?raw=true)

## Description 📑

The main goal of ``BanTech`` is to **consolidate** all your company's financial information into one place, with an easy way of linking your bank accounts into our app.
Once you have created your BanTech account and linked your bank accounts, you could see all your bank's metrics in our practical Dashboard.

BanTech is a solution of **open banking**. We decided to focus our app on companies because they usually have lots of bank accounts and face the challenges of trying to
consolidate bank information into typically an **excel**, our solution can solve this "excel problem". For the moment we support only banks in Uruguay.

To solve this problem we use a third-party ``API`` (Application Programming Interface) --> [Datanomik](https://www.datanomik.com/en/).
This API allows us to link your bank accounts to our app, we trust Datanomik because they complied with all the [security standards](https://docs.datanomik.com/docs/about-security).

## Installation 💻

**Environment**: ``Ubuntu LTS 20.04``

#### First you need to clone this repo:

```
git clone https://github.com/JuanManuelReyes/bantech-mvp.git
```

#### Second install the following dependencies with ``pip``:

```
autopep8==1.5.7
click==8.0.1
colorama==0.4.4
Flask==2.0.1
Flask-Login==0.5.0
Flask-MySQLdb==0.2.0
Flask-WTF==0.15.1
itsdangerous==2.0.1
Jinja2==3.0.1
MarkupSafe==2.0.1
mysqlclient==2.0.3
pycodestyle==2.7.0
toml==0.10.2
Werkzeug==2.0.1
WTForms==2.3.3
```

#### Third install Database:

You need to install ``MySQL`` and run the following script (this script is in the **flask_server** folder):

```
cat script-database.sql | sudo mysql -uroot -p
```
Once you enter your password the script will create the database and populate some users data.

#### Execute **backend**:

```
python flask_server/src/app.py
```

#### Execute **front-end**:

You need to go to **client** folder and execute the following commands

```
apt-get install node
npm install
npm start
```

## Demo video of the app:

[![Alt text](https://img.youtube.com/vi/OKHy-u2kb8M/0.jpg)](https://www.youtube.com/watch?v=OKHy-u2kb8M)

## Features 🥇

We implemented the following features:

* Create an account
* Link all your bank accounts
* Delete bank accounts
* Visualize all your bank transactions in one place
* Visualize consolidated metrics of your bank information in our Dashboard

## Future Features 🚀

In the future we would like to add the following features:

* Support banks from other countries
* Create our own ``API scrapping`` to link bank accounts instead of using Datanomik
* Add an **Analytics** page with custom metrics
* Artificial Intelligence
* Different permissions by user

## Tecnologies :computer:

#### Front-end:

* React
* HTML
* CSS
* JavaScript

#### Back-end:

* Python
* Flask
> Note - modules used in Flask: flask, flask_login, flask_session, flask_cors, flask_mysqldb, flask_wtf.csrf
* MySQL (for the databased)

#### API's:
* [Datanomik API](https://docs.datanomik.com/docs/overview-1)
* [BROU quotes](https://github.com/gmanriqueUy/cotizaciones-brou)

#### Other tools:

* Github
* Figma
* Trello

## Authors :pen:

* [Agustin Flom](https://www.linkedin.com/in/agustin-f/)
* [Juan Manuel Reyes](https://www.linkedin.com/in/juanma-reyess/)
* [Marcel Carrasco](https://www.linkedin.com/in/marcela-carrasco-piaggio-0796b333/)
* [Tarik Calixto](https://www.linkedin.com/in/tarik-calixto-964b52b5/)

## Licence :lock:

This project is published only for educational purposes. It must not be distributed without permission of the authors.
