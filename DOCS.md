sudo apt-get install nginx
verify nginx
sudo nginx -v
sudo apt-get install mariadb-server
sudo apt-get update
sudo apt-get install php7.2-fpm
sudo apt-get install php7.2
sudo apt-get install mariadb-client
sudo systemctl enable nginx
sudo systemctl start nginx
sudo systemctl status nginx
sudo systemctl enable mariadb
sudo systemctl start mariadb
sudo systemctl status mariadb
sudo mysql_secure_installation
Answer all yes (y)
In browser type /etc/nginx/sites-available/
Duplicate the default.txt file and rename to midtest.txt
nano midtest.txt
sudo systemctl enable php7.2-fpm
sudo systemctl status php7.2-fpm
nano midtest.txt
mv midtest.txt midtest
nano midtest
Change in line 22 to listen 80; only
Change in line 23 to listen [::]80; only
Add index.php in line 44 right berfore index.html
Uncomment the location ~ \.php$ block from line 56 to 63
Change FPM version from 7.0 to 7.2
Uncomment the location ~ /\.ht block from line 68 to 70
Exit midtest
sudo nginx -t
Successful
Type sudo ln -s /etc/nginx/sites-available/midtest /etc/nginx/sites-enabled/
Type sudo unlink /etc/nginx/sites-enabled/default
Move the file midtest to /etc/nginx/sites-available/
sudo mv midtest /etc/nginx/sites-available/
sudo ln -s /etc/nginx/sites-available/midtest /etc/nginx/sites-enabled/
cd /etc/nignx/sites-available/
nano midtest
Keep the PHP-CGI line commented
Exit midtest
sudo nginx -t
Success
sudo systemctl reload nginx
cd /var/www/html/
sudo nano info.php
Open browser type localhost/info.php
Delete the info file using sudo rm info.php
cd .
Type sudo wget unzip http://lionwiki.0o.cz/download/3.2.11/lionwiki-3.2.11.zip
Type unzip lionwiki-3.2.11.zip
Erase listen[::]80; from midtest
sudo ngnix -t
sudo systemctl reload nginx
Open terminal in lionwiki-3.2.11 folder
Move all the files to /var/www/html
Open browser type localhost/index.php
Edit main page
Add [] to create links for information
sudo chmod 7 var
Edit sub pages
Save changes after answering the 2 question
Upload files to github
sudo apt install git
sudo git commit
sudo git add var
sudo git pull origin master
sudo git push origin master
