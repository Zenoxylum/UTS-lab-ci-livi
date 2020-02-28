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
Type sudo ln -s/etc/nginx/sites-available/midtest /etc/nginx/sites-enabled/
Type sudo unlink /etc/nginx/sites-enabled/default
Move the file midtest to /etc/nginx/sites-available/
