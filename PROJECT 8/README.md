# IMPLEMENTING LOAD BALANCERS WITH NGINX AND SHELL SCRIPTING FOR AUTOMATION

Sequel to the previous project on load balancing with nginx, this project uses shell scripting to automate the processes of updating, installing software, addresses and ports configuration.

# STEP SUMMARY

Two instances are launched on AWS and apache webserver installed on them with shell scripting. An instance for the nginx load balancer.The first image below depicts the shell that runs the installation of apache webserver and the html page to be displayed if successful. 

![Alt text](<images/Screenshot 2024-02-22 at 10.32.12.png>)

To verify the load balancing is set up, the nginx address will display the public address of the apache webservers as seen in the images below. 

# Webserver-1
![Alt text](<images/Screenshot 2024-02-22 at 10.39.04.png>)

# Webserver-2
![Alt text](<images/Screenshot 2024-02-22 at 10.41.01.png>)

# Nginx server
![Alt text](<images/Screenshot 2024-02-22 at 10.42.21.png>)