- Install Apache|PHP|MySQL
- Step 1: Install and Set up Apache
- Open CMD select run as Administrator
- cd C:\Apache24\bin =>Enter
- parse:  httpd -k install =>Enter
- Open C:\Apache24\conf\httpd.conf
- Remove # at ServerName www.example.com:80 => Restart
- Remove # at LoadModule rewrite_module modules/mod_rewrite.so => Restart
- Search All AllowOverride None changes AllowOverride All
- if want Apache on service need Open CMD select run as Administrator
- parse: sc delete Apache2.4


