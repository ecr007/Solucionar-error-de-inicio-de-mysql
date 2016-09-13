# Solucionar-error-de-inicio-de-mysql
Solucionar error de inicio en linux
```
sudo service mysql stop

sudo rm /var/lib/mysql/ib_logfile0
sudo rm /var/lib/mysql/ib_logfile1

and comment out the line record_buffer=64M in /etc/mysql/my.cnf [1]

and then restart msyql using:

sudo service mysql restart
```
