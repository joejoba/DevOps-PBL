# LEMP IMPLEMENTATION

LEMP - Linux, Nginx, MySQL, PHP or Python

## PREREQUISITES
- AWS ACCOUNT 
- CREATING AND CONNECTING TO EC2 INSTANCE 
- KNOWLEDGE OF LINUX

## STEP 1 - CONNECTION TO EC2 USING TERMINAL 

Using the private key generated from the creation of the EC2 instance, the private key and the ip address are used to connect the server to the terminal on a computer. 

## STEP 2 - INSTALLING NGINX

Nginx is a web server software. With the server running, an update on the server is required. Nginx is installed using the `sudo apt install nginx` command as seen in image below.

![Alt text](<images/Nginx Installation.png>)

It is important to confirm the active status of the nginx running using `sudo systemctl status nginx` command as seen in the image below.

![Alt text](<images/Nginx Status.png>)

The Nginx server is tested using the `curl` command as port 80 has been enabled. The below image shows that nginx has been correctly installed and working.

![Alt text](<images/Nginx Curl.png>)

## STEP 3 - INSTALLING MySQL

MySQL is a relational database to store data. This is installed on the server using the `sudo apt install mysql-server` command as seen in the image below.

![Alt text](<images/Nginx MySql Installation.png>)

It is esential to provide a new password to this database as an administrator, for security reasons. Using the MySQL shell, an interactive script is provided to run password validation as seen in the image below.

![Alt text](<images/Mysql Password Validation.png>)

## STEP 3 - INSTALLING PHP

PHP is the setup that processes the code that is diplayed to the user as content. This is installed using the ``sudo apt install php-fpm php-mysql` command as seen in the image below.

![Alt text](<images/Nginx Php Installation.png>)

## STEP 4 - CONFIGURING NGINX TO USE PHP PROCESSOR

A directory is created as the root folder to store a html file. A .conf file is created in the sites-available folder, which is linked to sites-enabled folder to render the expected page. The default nginx sites-enabled file is unlinked, the hello message is passed to the html file and expected to be rendered to the web page as seen in the image below.

![Alt text](<images/Configuring Nginx to use PHP Processor.png>)

Result from the web page is evidenced below.

![Alt text](<images/Configuring Nginx for PHP 2.png>)