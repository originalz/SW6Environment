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
### Switch PHP Version for php cli
```bash
mkdir ~/bin && cd ~/bin
```
```bash
ln -s /usr/local/php8.0/bin/php php
```
```bash
echo 'PATH=$HOME/bin:$PATH' >> ~/.bash_profile
```
```bash
source ~/.bash_profile
```
