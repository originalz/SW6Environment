### PHP location plesk server and memory limit parameter
```bash
remote server  > /opt/plesk/php/7.4/bin/php -d memory_limit=-1
```
### User creation with console
```bash
remote server  > bin/console user:create --admin --email=keanu.klenner@connectiv.de --firstName="keanu" --lastName="klenner" --password=connectiv --no-interaction keanuklenner
```
### Available Shopware 6 Page Events
#### The events can be found in your vendor directory
```bash
vendor/shopware/core/Content/ContentName/...Event.php
```
### Additional information about .htaccess
#### Location of the .htaccess and password file
```bash 
shopware_root/public
```
#### How to force disable pwd protection
```bash
satisfy Any
```
### Additional information about messagequeues
The table "dead_message" denies some tasks in the messagequeue to get scheduled. You have to remove the dead message and reset the task manually to scheduled again.
