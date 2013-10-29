#DrupalDev nginx

Master - <img src="http://r2.ayil.co.uk:8080/buildStatus/icon?job=drupaldev-nginx-master">
Dev - <img src="http://r2.ayil.co.uk:8080/buildStatus/icon?job=drupaldev-nginx-dev">

Modified vagrant config from puphpet. Supports Drupal 6/7/8. Built in Drush and Composer.

#Tools
1. Removed xhprof it doesn't work in this config
2. Easier handling of vhosts and dbs (see example.pp)
3. Drush
4. Compass
5. Omega 4 Gems included as standard
6. APC / Memcache
7. Mailcatcher - run `mailcatcher --ip=0.0.0.0` / access example.drupal.dev:1080

#Dependencies
* Xcode with Command Line Tools installed
* Vagrant - http://www.vagrantup.com/
* VirtualBox - https://www.virtualbox.org/

#Install

1. Clone Me
2. `cd drupaldev-nginx`
3. `mkdir sites`
4. `cp manifests/example.pp manifests/devsites.pp`
5. Amend manifests/devsites.pp as required to desired server/virtualhost name and db details
6. `vagrant up`

#VM Info
* Default port 33.33.33.10
* Sites built as *.drupal.dev (use dnsmasq)
* Ubuntu 12.04

