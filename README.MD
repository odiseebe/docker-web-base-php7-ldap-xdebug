# Xdebug addon for Docker CentOS7 / Apache / PHP7 / LDAP base

## Description
Xdebug addon dockerfile a CentOS7 / Apache / PHP7 / LDAP docker container for local development purpose

## Specifications
### In the base container
* CentOS 7.4.1708
* Apache webserver (httpd)
* PHP7 (http://rpms.remirepo.net/enterprise/remi-release-7.rpm)
* LDAP
### Addon with this dockerfile
* Xdebug

## How to use
### Configuration variables
* VOLUME (/var/www/html)
* PORTS (80)

### Example
docker run -ti -p 8080:80 -v /host/path:/var/www/html --name test-base odisee/web-base-php7-xdebug