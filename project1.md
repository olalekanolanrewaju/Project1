# Documentation of Project 1
## Step 1
   ### Task 1: update a list of packages in package manager
   `sudo apt update`
   
   ![output ](./Images/output%20sudo%20apt%20update.png)
### Task 2: run apache2 package installation
`sudo apt install apache2`
 ![alt text](./Images/output%20sudo%20apt%20install%20apache2.png)
### Task 3: To verify that apache2 is running as a Service in our OS
`sudo systemctl status apache2`
 ![alt text](./Images/output%20apache%20service%20verification.png)
### Server is now running and can be accessed locally and externally

### To access locally, use the command below;
`curl` http://localhost:80
 ![alt text](./Images/output%20of%20local%20access.png)
### To access externally, use the command below;
`curl` http://18.209.19.218:80
 ![alt text](./Images/output%20of%20public%20access.png)
## Step 2

#INSTALLING MYSQL

### Use the command below to install MYSQL Server
`sudo apt install mysql-server`
 ![alt text](./Images/output%20MYSQL%20Server%20installation.png)
### Use the command below to logon to MYSQL
`sudo mysql`
 ![alt text](./Images/Output%20MYSQL%20Connection.png)
### It is important to run the security key that comes preinstalled with MYSQL to remove insecurities and lock down access to database.

### Before running the script,a password is required for the root user, using mysql_native_password as default authentication method. Password will be defined as PassWord.1.

### Use the command below to set the password
`ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'PassWord.1';`
 ![alt text](./Images/Out%20of%20password%20set%20for%20root%20user.png)
### Exit MYSQL Shell with the command below
`exit`
### The interactive script can be started by running the command below
`sudo mysql_secure_installation`

### This will ask if you want to configure the VALIDATE PASSWORD PLUGIN.

Note: Enabling this feature is something of a judgment call. If enabled, passwords which don’t match the specified criteria will be rejected by MySQL with an error. It is safe to leave validation disabled, but you should always use strong, unique passwords for database credentials.

Answer Y for yes, or anything else to continue without enabling.

### Test connectivity with the root to MYSQL with the command below
 `sudo mysql -p`

## Step 3
## Installing PHP

###  PHP is the component of our setup that will process code to display dynamic content to the end user. In addition to the php package, you’ll need php-mysql, a PHP module that allows PHP to communicate with MySQL-based databases. 

### To install these 3 packages at once, run: the command below
`sudo apt install php libapache2-mod-php php-mysql`
### To confirm PHP version, use this the command below;
`php -v`
### At this point, your LAMP stack is completely installed and fully operational.
### Linux (Ubuntu)
### Apache HTTP Server
### MySQL
### PHP

### STEP 4 — CREATING A VIRTUAL HOST FOR YOUR WEBSITE USING APACHE


#### I dont seem to understand from the PHP bit...I need some clarity











