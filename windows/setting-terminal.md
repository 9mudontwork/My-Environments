# Setup Terminal

## Starship

{% embed url="https://starship.rs/" %}

## Windows Terminal

ถ้ายังไม่มี Profiles ให้สร้าง

```javascript
if (!(Test-Path -Path $PROFILE )){ New-Item -Type File -Path $PROFILE -Force }

ไฟล์จะอยู่ที่ C:\Users\i3acksp4ce\Documents\WindowsPowerShell

ใส่ 
Invoke-Expression (&starship init powershell)
```

### Settings Profiles

```javascript
"colorScheme": "My Color",
"cursorColor": "#FFFFFF",
"cursorShape": "bar",
"fontFace": "Fira Code",
"acrylicOpacity": 0.7,
"closeOnExit": true,
"fontSize": 14,
"snapOnInput": true,
"useAcrylic": true,
"startingDirectory": "."

"schemes": [
    {
        "name" : "My Color",
    
        "cursorColor": "#C5C8C6",
        "selectionBackground": "#C5C8C6",
    
        "background" : "#1D1F21",
        "foreground" : "#ffffff",
    
        "black" : "#1D1F21",
        "blue" : "#399ced",
        "cyan" : "#3971ED",
        "green" : "#198844",
        "purple" : "#A36AC7",
        "red" : "#CC342B",
        "white" : "#C5C8C6",
        "yellow" : "#FBA922",
        "brightBlack" : "#969896",
        "brightBlue" : "#3971ED",
        "brightCyan" : "#3971ED",
        "brightGreen" : "#198844",
        "brightPurple" : "#A36AC7",
        "brightRed" : "#CC342B",
        "brightWhite" : "#FFFFFF",
        "brightYellow" : "#FBA922"
    }
],
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

คลิกขวา new -&gt; string value \(ตั้งชื่อว่า icon\)

```javascript
%USERPROFILE%/AppData/Local/WTerminal/terminal.ico
```

