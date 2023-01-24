## Shopware 6 General Information
### .htaccess
#### Location of the .htaccess and password file
```bash 
shopware_root/public
```
#### How to force disable pwd protection
```bash
satisfy Any
```
### MessageQueue
The table "dead_message" denies some tasks in the messagequeue to get scheduled. You have to remove the dead message and reset the task manually to scheduled again.
