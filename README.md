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
