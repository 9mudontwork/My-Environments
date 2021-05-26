# Exmaple Config

```text
<VirtualHost *:80> 
    DocumentRoot "C:/Users/i3acksp4ce/Desktop/projects/diversition/tcint/frontend/web/"
    ServerName tcint.test
    ServerAlias *.tcint.test
    <Directory "C:/Users/i3acksp4ce/Desktop/projects/diversition/tcint/frontend/web/">
        AllowOverride All
        Require all granted

        RewriteEngine on
        RewriteCond %{REQUEST_FILENAME} !-f
        RewriteCond %{REQUEST_FILENAME} !-d
        RewriteRule . index.php
    </Directory>

    Alias /admin C:/Users/i3acksp4ce/Desktop/projects/diversition/tcint/backend/web/
    RewriteRule ^/admin$ /admin/ [L,PT]

    <Directory "C:/Users/i3acksp4ce/Desktop/projects/diversition/tcint/backend/web/">
        AllowOverride All
        Require all granted

        RewriteEngine on
        RewriteCond %{REQUEST_FILENAME} !-f
        RewriteCond %{REQUEST_FILENAME} !-d
        RewriteRule . index.php
    </Directory>
</VirtualHost>

# If you want to use SSL, enable it by going to Menu > Apache > SSL > Enabled
```

