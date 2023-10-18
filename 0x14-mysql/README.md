0x14. MySQL
---
For both web-01 and web-02 servers:
SSH into the server as usual:

bash
Copy code
ssh ubuntu@<server-ip>
Update the package list:

bash
Copy code
sudo apt update
Download and add the MySQL APT repository package:

bash
Copy code
sudo apt-get install software-properties-common
sudo add-apt-repository 'deb http://archive.ubuntu.com/ubuntu xenial universe'
Update the package list again:

bash
Copy code
sudo apt update
Install MySQL 5.7:

bash
Copy code
sudo apt install mysql-server-5.7
During the installation, you will be prompted to set a password for the MySQL root user. Follow the prompts to set a secure password.

Enable and start the MySQL service:

bash
Copy code
sudo systemctl enable mysql
sudo systemctl start mysql
Check the MySQL version:

bash
Copy code
mysql --version

By following these steps, you should be able to successfully install MySQL 5.7 on your web-01 and web-02 servers.
