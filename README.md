## Documentation of project1

`sudo apt update`

`sudo apt install apache2`

`sudo systemctl status apache2`

![apache status running](./images/apache.png)

`testing the apache2` 
![apache default page](./images/apachepage.png)

`sudo apt install mysql-server`
![mysqlserver running](./images/mysql.png)

`ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'PassWord.1';`

`mysql> exit`

`sudo mysql_secure_installation`
![password](.images/mysqlpassword.png)

`mysql> exit`

`sudo apt install php libapache2-mod-php php-mysql`

`sudo mkdir /var/www/projectlamp`

`sudo chown -R $USER:$USER /var/www/projectlamp`

`sudo vi /etc/apache2/sites-available/projectlamp.conf`

`sudo ls /etc/apache2/sites-available`

`sudo a2ensite projectlamp`

`sudo apache2ctl configtest`

`sudo systemctl reload apache2`

![http://<Public-IP-Address>:80](.images/hellolamp.png)

`sudo vim /etc/apache2/mods-enabled/dir.conf`

`sudo systemctl reload apache2`


