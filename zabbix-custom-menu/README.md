In this example we create a new menu in Zabbix frontend pointing to a custom PHP page - Hello World. 

INSTALLATION:
You can just copy all files into root UI zabbix frontend directory (usually /usr/share/webapps/zabbix)

How it works?
1. Edit include/menu.inc.php to add a new CMenuItem calling 'Hello World' having setUrl pointing to desired page 
2. Edit include/classes/mvc/CRouter.php and find $routes section to add CLegacyAction.

There is always .bak file containing original stock Zabbix file. 
This example was done on version 5.0.2-1.
If you have newer Zabbix version  then take a look on .diff file where to adjust your file accordingly.
In case of another major Zabbix version and overwrite stock file you are in risk of loose integrity.

Best Regards
Heksik - Zabbix guru

