# LAMP IMPLEMENTATION

LAMP - Linux, Apache, MySQL, PHP or Python

## PREREQUISITES
- AWS ACCOUNT 
- CREATING AND CONNECTING TO EC2 INSTANCE 
- KNOWLEDGE OF LINUX

## STEP 1 - CONNECTION TO EC2 USING TERMINAL 

Using the private key generated from the creation of the EC2 instance, the private key and the ip address are used to connect the server to the terminal on a computer. 

## STEP 2 - IINSTALLING APACHE

Apache is a web server HTTP server software. With the server running, an update on the server is required. Apache is installed using the `sudo apt install apache2` command as seen in image below.

![Alt text](<images/Apache Installation.png>)

It is important to check the status of the apache running using `sudo systemctl status apache2` command as seen in the image below.

![Alt text](<images/Apache status.png>)

The Apache server is tested using the `curl` command as port 80 has been enabled. The below image shows that apache has been correctly installed and working.

![Alt text](<images/Apache works.png>)

## STEP 3 - INSTALLING MySQL

MySQL is a relational database to store data. This is installed on the server using the `sudo apt install mysql-server` command as seen in the image below.

![Alt text](<images/Mysql Installation.png>)

It is esential to provide a new password to this database as an administrator, for security reasons. Using the MySQL shell, an interactive script is provided to run password validation as seen in the image below.

![Alt text](<images/Mysql Password Validation.png>)

## STEP 3 - INSTALLING PHP

PHP is the setup that processes the code that is diplayed to the user as content. This is installed using the ``sudo apt install php libapache2-mod-php php-mysql` command as seen in the image below.

![Alt text](<images/Php Installation.png>)

With the modification of the precedence, the index.php file is ranked before the index.html file to display the info page of php on the web browser as seen in the image below. 

![Alt text](<images/PHP Version.png>)

## STEP 4 - VIRTUAL HOST USING APACHE

A .conf file is created in the configuration folder of apache to render a webpage. Disabling ther default apache page to render the new file we passed on to be displayed as seen in the image below.

![Alt text](<images/Creating Virtual Host Using Apache.png>)

The message passed on is displayed on the webpage as seen in the image below. 

![Alt text](<images/Virtual Host Setup with Apache.png>)