<h1 style="font-size:10vw" align="center">Windows Privilege Escalation</h1>
<h2 style="font-size:7vw" align="center"><i> Exploit for CVE-2021-1732 (Win32k) - Local Privilege Escalation</i></h2>
*For educational and authorized security research purposes only*

## Original Exploit Authors
[@Exploit Blizzard](https://github.com/exploitblizzard)

## Vulnerability Description
A vulnerability exists within win32k that can be leveraged by an attacker to escalate privileges to those of NT AUTHORITY\SYSTEM. The flaw exists in how the WndExtra field of a window can be manipulated into being treated as an offset despite being populated by an attacker-controlled value. This can be leveraged to achieve an out of bounds write operation, eventually leading to privilege escalation. This flaw was originally identified as CVE-2021-1732 and was patched by Microsoft on February 9th, 2021. In early 2022.

## Usage
```bash
  CVE-2021-1732.exe "the-command"
```

## Options
```bash
  "the-command"    Use every command supported by Command Line Interfaces (CLI), such as "whoami"
```

## Download Via Original Source
[Download Exploit Script for CVE-2021-3560 Here](https://raw.githubusercontent.com/UNICORDev/exploit-CVE-2021-3560/main/exploit-CVE-2021-3560.py)

## Exploit Requirements
- Command Prompt
- Proccess Hacker

## Demo
![Animation1](https://github.com/asepsaepdin/CVE-2021-1732/assets/122620685/f6437f0b-3598-4833-b34d-354241bf9322)

## Tested On
- Windows 10 Version 2004

## Affected Windows Versions:
Windows Server, version 20H2 (Server Core Installation), Windows 10 Version 20H2, Windows Server, version 2004 (Server Core installation), Windows 10 Version 2004, Windows Server, version 1909 (Server Core installation), Windows 10 Version 1909, Windows Server 2019 (Server Core installation), Windows Server 2019, Windows 10 Version 1809
***

## Warning
⚠️ Becareful when running this exploit on your system.

## Credits
- https://nvd.nist.gov/vuln/detail/cve-2021-1732
- https://bbs.kanxue.com/thread-266362.html
- https://github.com/exploitblizzard/Windows-Privilege-Escalation-CVE-2021-1732
- https://packetstormsecurity.com/files/166169/Win32k-ConsoleControl-Offset-Confusion-Privilege-Escalation.html
