
#### Author: Aysad Kozanoglu
##### Email: aysadx@gmail.com

my one-liner auto installer scripts for debian Jessie (jessie LTS until 2020) stretch  (and derivates like ubuntu)

##### MariaDB singler Server installation
[source](https://github.com/AysadKozanoglu/scripts/blob/master/mariadb-install.sh)
```
wget -O - https://git.io/fjWjB | bash
```

##### nginx threads,iao, stream, ssl compile installation
[source](https://github.com/AysadKozanoglu/scripts/blob/master/nginx-compile.sh)
```
wget -O - https://git.io/JvLnJ| bash
```

##### php7.2 installation
[source](https://github.com/AysadKozanoglu/scripts/blob/master/php7.2-install.sh)
```
wget -O - https://git.io/JvLZx | bash
```
##### KVM CLoud with WEB Gui installation
[source](https://github.com/AysadKozanoglu/webvirtmgr/wiki/Install-WebVirtMgr-KVM-Cloud---Easy-auto-installer)
```
wget -O part1.sh https://git.io/fpAJH && sh part1.sh
wget -O part2.sh https://git.io/fpAJA && sh part2.sh
/var/www/webvirtmgr/manage.py syncdb
/var/www/webvirtmgr/manage.py collectstatic
chown -R www-data:www-data /var/www/webvirtmgr
sudo  -u www-data bash -c "/usr/bin/python /var/www/webvirtmgr/console/webvirtmgr-console >> /var/www/webvirtmgr/webService.log 2>&1 &" 
sudo  -u www-data bash -c "/usr/bin/python /var/www/webvirtmgr/manage.py runserver 127.0.0.1:8000 >> /var/www/webvirtmgr/webService.log 2>&1 & "
```
##### XEN Orchestra Community Edition from source installation
[source](https://raw.githubusercontent.com/AysadKozanoglu/Auto-installer-xen-orchestra-source/master/xo-auto-installer.sh)
```
wget -O -  https://git.io/fhIr6 | bash
```

