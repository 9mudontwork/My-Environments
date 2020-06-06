# Setting Terminal

## Starship

{% embed url="https://starship.rs/" %}

## Windows Terminal

ถ้ายังไม่มี Profiles ให้สร้าง

```javascript
if (!(Test-Path -Path $PROFILE ))
{ New-Item -Type File -Path $PROFILE -Force }
```

### Settings Profiles

```javascript
"hidden": false,
"colorScheme": "One Half Dark",
"cursorColor": "#FFFFFF",
"cursorShape": "bar",
"fontFace": "Fira Code",
"acrylicOpacity": 0.7,
"closeOnExit": true,
"fontSize": 14,
"snapOnInput": true,
"useAcrylic": true,
"startingDirectory": "."
```

### Right Click Context menu

สร้างไฟล์นามสกุล .reg

```javascript
Windows Registry Editor Version 5.00

[HKEY_CLASSES_ROOT\Directory\Background\shell\wt]
 @="Open Windows Terminal here"

[HKEY_CLASSES_ROOT\Directory\Background\shell\wt\command]
 @="C:\\Users\\<UserName>\\AppData\\Local\\Microsoft\\WindowsApps\\wt.exe"
```

เปิด Run

```javascript
%USERPROFILE%/AppData/Local/
```

สร้าง Folder

```javascript
WTerminal
```

เอา Icon ไปใส่

{% file src="../.gitbook/assets/terminal.ico" caption="Windows Terminal Icon" %}

เปิด Registry Editor แล้วไปที่

```javascript
HKEY_CLASSES_ROOT\Directory\Background\shell\wt
```

คลิกขวา new -&gt; string value

```javascript
%USERPROFILE%/AppData/Local/WTerminal/terminal.ico
```

