# Exmaple Config

```text
<VirtualHost *:80> 
    DocumentRoot "C:/Users/i3acksp4ce/Desktop/INNOC/frontend/web/"
    ServerName f.innoc.test
    ServerAlias *.f.innoc.test
    <Directory "C:/Users/i3acksp4ce/Desktop/INNOC/frontend/web/">
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

