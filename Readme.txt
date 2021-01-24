ssl installation 
https://www.digitalocean.com/community/tutorials/how-to-secure-apache-with-let-s-encrypt-on-ubuntu-18-04

https://stackoverflow.com/questions/14927345/importerror-no-module-named-django-core-wsgi-apache-virtualenv-aws-wsgi

(run this command from home sometime from your system folder installation not work)
sudo apt-get remove libapache2-mod-python libapache2-mod-wsgi
sudo apt-get install libapache2-mod-wsgi-py3

agar fir bhi work na kre to 
envp activate krke ye run kre
mod_wsgi-express module-config

output ko /etc/apache2/apach2.conf me top pr likhe
pip install mod_wsgi 
after that 
/etc/apache2/apach2.conf me jao and nicke likhe line ko top pr past kr do 
apne virtualenv se path nikalkr
LoadModule wsgi_module "/var/www/html/envp/lib/python3.6/site-packages/mod_wsgi/server/mod_wsgi-py36.cpython-36m-x86_64-linux-gnu.so"


disble the default conf in  apache2 and create the new conf .
cd /etc/apache2/sites-available/

use /var/www/html/yourproject folder 

becouse some time you can face permission issue if you use other folder.


how to enbale config : sudo a2ensite virtual_host_file_name
how to disble config : sudo a2dissite virtual_host_file_name
