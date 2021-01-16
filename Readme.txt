ssl installation 
https://www.digitalocean.com/community/tutorials/how-to-secure-apache-with-let-s-encrypt-on-ubuntu-18-04

https://stackoverflow.com/questions/14927345/importerror-no-module-named-django-core-wsgi-apache-virtualenv-aws-wsgi

sudo apt-get remove libapache2-mod-python libapache2-mod-wsgi
sudo apt-get install libapache2-mod-wsgi-py3



disble the default conf in  apache2 and create the new conf .
cd /etc/apache2/sites-available/

use /var/www/html/yourproject folder 

becouse some time you can face permission issue if you use other folder.
