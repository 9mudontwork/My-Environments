# Setup Terminal

## Starship

ติดตั้งตาม document

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
"initialCols": 70,
"initialRows": 20,

"profiles": {
		"defaults": {
			// Put settings here that you want to apply to all profiles.
			"fontFace": "FiraCode NF",
			"acrylicOpacity": 0.9,
			"closeOnExit": true,
			"fontSize": 14,
			"snapOnInput": true,
			"useAcrylic": true,
			"startingDirectory": ".",
			"colorScheme": "MyColor"
		},

// Add custom color schemes to this array.
// To learn more about color schemes, visit https://aka.ms/terminal-color-schemes
	"schemes": [
		{
			"name": "My Color",

			"cursorColor": "#C5C8C6",
			"selectionBackground": "#C5C8C6",

			"background": "#0D1117",
			"foreground": "#F0F6FC",

			"black": "#1D1F21",
			"blue": "#399ced",
			"cyan": "#388BFD",
			"green": "#3FB950",
			"purple": "#6E40C9",
			"red": "#DA3633",
			"white": "#C5C8C6",
			"yellow": "#E3B341",
			"brightBlack": "#969896",
			"brightBlue": "#388BFD",
			"brightCyan": "#388BFD",
			"brightGreen": "#3FB950",
			"brightPurple": "#6E40C9",
			"brightRed": "#DA3633",
			"brightWhite": "#FFFFFF",
			"brightYellow": "#E3B341"
		}
	],
	
	
	
	// custom color
	{
            "background": "#0D1117",
            "black": "#1D1F21",
            "blue": "#399CED",
            "brightBlack": "#969896",
            "brightBlue": "#388BFD",
            "brightCyan": "#388BFD",
            "brightGreen": "#3FB950",
            "brightPurple": "#6E40C9",
            "brightRed": "#DA3633",
            "brightWhite": "#FFFFFF",
            "brightYellow": "#E3B341",
            "cursorColor": "#C5C8C6",
            "cyan": "#388BFD",
            "foreground": "#F0F6FC",
            "green": "#3FB950",
            "name": "MyColor",
            "purple": "#6E40C9",
            "red": "#DA3633",
            "selectionBackground": "#C5C8C6",
            "white": "#C5C8C6",
            "yellow": "#E3B341"
        },
        
//ให้อยู่ตรงกลางตอนเปิด
"centerOnLaunch": true,
```

### Right Click Context menu

สร้างไฟล์นามสกุล .reg

```javascript
Windows Registry Editor Version 5.00

[HKEY_CLASSES_ROOT\Directory\Background\shell\wt]
 @="Open Windows Terminal here"

[HKEY_CLASSES_ROOT\Directory\Background\shell\wt\command]
 @="C:\\Users\\i3acksp4ce\\AppData\\Local\\Microsoft\\WindowsApps\\wt.exe"
```

{% file src="../../.gitbook/assets/register-wt.txt" caption="register window terminal" %}

เปิด Run

```javascript
%USERPROFILE%/AppData/Local/
```

สร้าง Folder

```javascript
WTerminal
```

เอา Icon ไปใส่

{% file src="../../.gitbook/assets/terminal.ico" caption="Windows Terminal Icon" %}

เปิด Registry Editor แล้วไปที่

```javascript
HKEY_CLASSES_ROOT\Directory\Background\shell\wt
```

คลิกขวา new -&gt; string value \(ตั้งชื่อว่า icon\)

```javascript
%USERPROFILE%/AppData/Local/WTerminal/terminal.ico
```

