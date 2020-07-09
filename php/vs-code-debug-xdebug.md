# VS Code ทำ Debug ด้วย Xdebug

## ติดตั้ง extension

{% embed url="https://marketplace.visualstudio.com/items?itemName=felixfbecker.php-debug" %}

## ติดตั้ง Xdebug ให้ตรงกับ PHP Version ที่ลง

{% embed url="https://xdebug.org/download\#releases" %}

ย้ายไฟล์ php\_xdebug.dll ไปไว้ที่

```text
your-path\php\ext
```

เปิดไฟล์ php.ini แล้วเพิ่ม config

```text
zend_extension = "your-path\php\ext\php_xdebug.dll"

[XDebug]
xdebug.remote_enable = 1
xdebug.remote_autostart = 1 
```

