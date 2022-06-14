Provisioning a new site
=======================


##Required packages:
* nginx
* Python 3.9
* virtualenv + pip
* Git



eg, on Ubuntu:
sudo add-apt-repository ppa: fkrull/deadsnakes
sudo apt-get install nginx git python3.9 python3.9-venv

## Nginx virtual Host config
*see nginx.tenplate.conf
*replace SITENAME with,e.g., staging.my-domain.com
##Systend service
*see gunicorn-systend.tenplate.service
*replace SITENAME with, e.g., staging.my-domain.com

## Folder structure:
Assume we have a user account at /home/username
/home/username
- sites
    -SITENAME
        database
        source
        static
        virtualenv
