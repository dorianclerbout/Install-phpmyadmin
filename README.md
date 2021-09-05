# Install-phpmyadmin

- [1 - Install PHPMYADMIN packages ](#1---Install-PHPMYADMIN-packages) 
- [2 - Download PHPMYADMIN](#2---Download-PHPMYADMIN) 
- [3 -  Move PHPMYADMIN inside localhost](#3---Move-PHPMYADMIN-inside-localhost) 


## 1.  Install PHPMYADMIN packages


- php-mbstring: a PHP extension used to manage non-ASCII strings and convert strings to different encodings
-  php-zip: a PHP module that supports uploading .zip files to phpMyAdmin
    
- php-gd: another PHP module, this one enables support for the GD Graphics Library


       sudo apt install php-mbstring php-zip php-gd



## 2.  Download PHPMYADMIN

Inside Terminal :

    sudo apt-get install  phpmyadmin 

Reload Apache2 Server :

    sudo systemctl start apache2

## 3.  Move PHPMYADMIN inside localhost


    sudo ln -s /usr/share/phpmyadmin/var/www/html

and restart apache2  & start mysql:

    sudo systemctl restart apache2 
    sudo systemctl restart mysql 
 
