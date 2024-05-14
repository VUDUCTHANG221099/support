# Install Apache|PHP|MySQL
## Install Apache
1. link download: https://www.apachelounge.com/download/ [vs]
2. Remove comment at:  ServerName www.example.com:80
3. CMD run as Administrator: httpd -k install[install service]|sc delete Apache2.4
## Install PHP
1. link download: https://windows.php.net/download [win64]
2. php.ini-production|development => php.ini
3. Open php.ini
- URL: location ->ext in php
- Remove comment at: extension=curl
- Remove comment at: extension=mysqli
- Remove comment at: extension=gd
- Remove comment at: extension=mbstring
- Remove comment at: extension=pdo_mysql
- Remove comment at: extension=soap
- Remove comment at: extension=fileinfo
- Remove comment at: extension=zip
- Remove comment at: extension_dir = "ext" and change "ext"=>"URL\ext"
- Download cacert.pem save at: URL/extras/ssl
- URL-Cacert= "URL\extras\ssl\cacert.pem"
- Remove comment at: curl.cainfo = URL-Cacert
- Remove comment at: openssl.cafile= URL-Cacert
## Configuration apache and php
<!-- LoadModule php_module "URI-PHP\php8apache2_4.dll"
<FilesMatch \.php$>
    SetHandler application/x-httpd-php
</FilesMatch>
# configure the path to php.ini
PHPIniDir "URI-PHP" -->
- restart apache