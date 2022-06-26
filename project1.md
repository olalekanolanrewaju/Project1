# Documentation of Project 1
## Step 1
   ### Task 1: update a list of packages in package manager
   `sudo apt update`
### Task 2: run apache2 package installation
`sudo apt install apache2`

### Task 3: To verify that apache2 is running as a Service in our OS
`sudo systemctl status apache2`

### Server is now running and can be accessed locally and externally

### To access locally, use the command below;
`curl` http://localhost:80
### To access externally, use the command below;
`curl` http://18.209.19.218:80

## Step 2

#INSTALLING MYSQL

### Use the command below to install MYSQL Server
`sudo apt install mysql-server`

### Use the command below to logon to MYSQL
`sudo mysql`

### It is important to run the security key that comes preinstalled with MYSQL to remove insecurities and lock down access to database.

### Before running the script,a password is required for the root user, using mysql_native_password as default authentication method. Password will be defined as PassWord.1.

### Use the command below to set the password
`ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'PassWord.1';`
### Exit MYSQL Shell with the command below
`exit`
### The interactive script can be started by running the command below
`sudo mysql_secure_installation`

### This will ask if you want to configure the VALIDATE PASSWORD PLUGIN.

Note: Enabling this feature is something of a judgment call. If enabled, passwords which don’t match the specified criteria will be rejected by MySQL with an error. It is safe to leave validation disabled, but you should always use strong, unique passwords for database credentials.

Answer Y for yes, or anything else to continue without enabling.




