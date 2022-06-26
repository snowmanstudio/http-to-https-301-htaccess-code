# http-to-https-301-htaccess-code

RewriteEngine On

RewriteCond %{HTTPS} off

RewriteRule (.*) https://%{HTTP_HOST}%{REQUEST_URI} [R=301,L]

## To redirect using the 302 'temporarily moved' change [R=302,L]
