Provisioning a new site
=======================

## Required packages:

* nginx
* Python 3.8
* virtualenv + pip
* Git

eg, on Ubuntu:

    sudo apt update
    sudo apt-get install nginx git python3.8 python3.8-venv
    sudo apt-get install python3-pip

## Nginx Virtual Host config

* see nginx.template.conf
* replace SITENAME with, e.g., staging.my-domain.com

## Systemd service

* see gunicorn-systemd.template.service
* replace SITENAME with, e.g., staging.my-domain.com
* replace SEKRIT with email password

## Folder structure
Assume we have a user account at /home/username

/home/username
└── sites
    └── SITENAME
        ├── database
        ├── source
        ├── static
        └── virtualenv
