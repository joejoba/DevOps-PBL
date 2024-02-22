# IMPLEMENTING LOAD BALANCERS WITH NGINX

This project implements load balancing between two apache webservers to ensure high availiability to users. Nignx is the load balancer in use. 

## PREREQUISITES
- Access to a terminal 
- Knowledge of Linux
- AWS account, Apache and Nginx Installation

# STEPS SUMMARY
Two instances are created on AWS, apache webserver software installed on them to render webpages over the internet. The security configurations are set to listen on port 8000 as seen in the last two images below for both servers to allow traffic from anywhere. The servers are accessed through ssh to run commands. The default apache html is changed with a message "Welcome to my EC2 instance" and dispalyed on the webpage. A third instance is launched, nginx installed to act as the load balancer between the two apache webservers. The configuration file for nginx is edited showing the addresses and ports to enable load balancing of requests to the backend servers as seen in the first image below.

![Alt text](<images/Screenshot 2024-02-21 at 14.04.54.png>)

![Alt text](<images/Screenshot 2024-02-21 at 13.52.11.png>)

![Alt text](<images/Screenshot 2024-02-21 at 13.59.18.png>)
