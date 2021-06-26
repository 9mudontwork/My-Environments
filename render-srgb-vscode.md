# แก้ปัญหาการ render สี srgb ของ vscode

{% embed url="https://dev.to/iamst0rm/fixing-vscode-color-bug-on-linux-185f" %}



## Fixing VSCode Color Bug on Linux

[\#vscode](https://dev.to/t/vscode) [\#linux](https://dev.to/t/linux) [\#ubuntu](https://dev.to/t/ubuntu)[![](https://res.cloudinary.com/practicaldev/image/fetch/s--5nqDmOP9--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/458087/67d94e6d-ecfc-4047-a741-7c518a5a5e7e.jpeg)](https://dev.to/iamst0rm)Paras Verma31 ส.ค. 2563 ・_Updated on 17 พ.ค._ ・3 min read

Being a developer, I love VSCode. Using VSCode for a couple of years now, for Windows that is, was always a smooth sailing.  
PS. — I design and game too. So Windows is ❤

### Where the Problem began.

Shifted to Pop\_OS for a project, installed VSCode and as I began writing code, I noticed my editor tab having ‘multiple color blocks’. The blank area without any code/text had a different \(darker\) color than the area having the code/text.

[![Color Blocks in Text Editor](https://res.cloudinary.com/practicaldev/image/fetch/s--NJHBf2qe--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/i/qkf772nbdfhix37zv3q8.png)](https://res.cloudinary.com/practicaldev/image/fetch/s--NJHBf2qe--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/i/qkf772nbdfhix37zv3q8.png)

Putting computer to sleep and waking it introduced another issue. VSCode terminal and code preview areas were filled with noise… white noise. No metaphors here. Actual white noise.

[![White Noise](https://res.cloudinary.com/practicaldev/image/fetch/s--Q6f_jlMS--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/i/tx38phknicdieoofmwdd.jpeg)](https://res.cloudinary.com/practicaldev/image/fetch/s--Q6f_jlMS--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/i/tx38phknicdieoofmwdd.jpeg)

### Counter Checking with Windows

After this, I booted my Windows installation to check if its the new update but everything worked fine. No color blocks, no noisy white dots.

[![Windows VSCode](https://res.cloudinary.com/practicaldev/image/fetch/s--OukKsaJp--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/i/c4vf1745v4h6y8nnm9ht.png)](https://res.cloudinary.com/practicaldev/image/fetch/s--OukKsaJp--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/i/c4vf1745v4h6y8nnm9ht.png)

### What I found.

This Linux issue is occuring on almost all the distros I tried:

* Ubuntu 18.04 LTS
* Pop-OS 19.10 \(Nvidia and Intel/AMD\)
* Elementary OS
* Mint... and quite a few more.

### Why is it happening?

Though I figured out a fix, I couldn't figure out the depth of why or how it was occuring. It sure is related to how app on linux renders colors and color profile, as the fixes include color correct rendering and forcing a color profile.

If you find something else being the reason, please do respond to the post with your findings.

### The Solution. \(VSCode v1.43.x & Later\)

Microsoft is keen on messing with the solutions with every update. For now:

1. In VSCode, open Command Palette \(Ctrl+Shift+P\) and search for _**"Configure Runtime Arguments"**_. Select it and press **Enter**.
2. There should already be an entry:

`"disable-color-correct-rendering": true`

Just remove that entry or comment it out with //.

If there are any more entries, do remove those.

_**BOOM! Issue fixed.**_

For those of you, willing to read the whole process, here is a thorough compilation of the issue:  
[Link to my Medium story](https://medium.com/@iamstorm/vscode-bug-on-linux-7ca4c4544d24)

### Legacy/Older Solutions \(Work for versions earlier than 1.43.x\)

This issue is a weird rendering issue with VSCode on Linux. I found a very simple fix:

1. In VSCode, open Command Palette \(Ctrl+Shift+P\) and search for **"Configure Runtime Arguments"**. Select it and press Enter.
2. There should already be an entry:

`"disable-color-correct-rendering": true`

Add a comma \(,\) after this entry. Even if there is no entry, just put a code block \({}\) and follow along.

1. Paste in

`"disable-hardware-acceleration": true,`

\(in the next line, if there is already an entry\) inside the same code block.

1. Save the file. Restart VSCode

_**BOOM! Issue fixed.**_

[Link to original solution](https://github.com/microsoft/vscode/issues/85452#issuecomment-558334562).

#### Still Not Fixed?

The issue might still not be fixed for everyone \(as it wasn't for me\). Just follow along the steps:

1. Open Command Palette \(Ctrl+Shift+P\) and search for **"Configure Runtime Arguments"** and press Enter. Now just add this line at the end

`"force-color-profile": "srgb",`

It will display a zig-zag line underneath the entry and say **"Property force-color-profile is not allowed."**. Just ignore it and save the file.

1. Restart VSCode. Voila!!! Issue is fixed.

