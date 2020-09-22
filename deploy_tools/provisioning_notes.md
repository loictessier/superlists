Provisioning a new site
=======================

## Required packages:

* nginx
* Python 3.8
* pipenv (pip + virtualenv)
* Git

eg, on Ubuntu:

    sudo apt-get install nginx git python38
    sudo apt-get install python3-pip
    pip3 install pipenv

## Nginx Virtual Host config

* see nginx.template.conf
* replace SITENAME with, e.g., staging.my-domain.com

## Folder structure
Assume we have a user account at /home/username

/home/username
└── sites
    └── SITENAME
        ├── database
        ├── source
        ├── static
        └── virtualenv
