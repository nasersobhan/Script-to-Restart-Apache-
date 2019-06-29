# Shell Script to Restart Apache
Simple Bash Script to Restart Apache when it fails, 



this code is life saver, if you add it to your cron job (server) it checks the Apache and restart it if it not running and if you want you can add the mail notification option to have an email about it.

*/10 * * * * root /bin/bash /etc/scripts/apache_check.sh >> /etc/logs/apache_check.log 2>&1 #check apache
Above Cronjob Command Runs the script which is located in var/www/scripts/apache_check.sh every 10 minutes and save the result in apache_check.log in /etc/logs folder.
