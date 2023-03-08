## Shopware 6 Environment
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
### Plugin Snippets
If you want to add or change snippets in your plugin, you simply have to edit the snippet json file in
  - ```plugin/src/Resources/snippet/de_DE```

If you added new snippets or changed some, you have to execute: 
  - ```bin/console plugin:update pluginname --clearCache```
  - ```bin/console theme:compile```
