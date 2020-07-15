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
[XDebug]
zend_extension = "C:\xampp\php\ext\php_xdebug-2.9.6-7.2-vc15-x86_64.dll"
xdebug.idekey=VSCODE
xdebug.remote_enable = 1
xdebug.remote_autostart = 1 
```

## หรืออีกวิธี

สร้างไฟล์แสดง phpinfo\(\); แล้ว copy html code ไป analyze ที่เว็บ [https://xdebug.org/wizard](https://xdebug.org/wizard) แล้วทำตามขั้นตอน

## ใช้ กับ postman

เพิ่ม params 

```text
?XDEBUG_SESSION_START=VSCODE
```

