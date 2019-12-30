# NagiosConfiguration
Nagios Configuration

Configuration services and hosts
```ssh
vim /etc/nagios/objects/localhost.cfg
service nagios restart
```
Naggios commands declaration for services
```sh
vim /etc/nagios/objects/commands.cfg
```
Scripts of check
```sh
vim /usr/lib64/nagios/plugins/check_hddssh
```
Script exec under Nagios user:
```sh
su nagios -c '/usr/lib64/nagios/plugins/check_hddssh ***HOST** root ***PASS*** 22'
```
Nagios Graph errors:
```sh
tail -300 /var/nagiosgraph/nagiosgraph.log

vim /etc/nagiosgraph/map
```
Error test:
```sh
nagios -v /etc/nagios/nagios.cfg
```
