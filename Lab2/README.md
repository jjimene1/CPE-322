# Lab 2 - Raspberry Pi and Command Shell

## Lab Commands: Execution and Output

As part of the lab we are going to execute some terminal commands, display their output on my local machine, and we are going to define their function based on these outputs:

### hostname

```bash
$ hostname
DESKTOP-JQOE2UL
```

This command displays the current host, domain, or node name of the system. It uniquely identifies a computer in a network.

### env

```bash

$ env
!::=::\
CommonProgramFiles(x86)=C:\Program Files (x86)\Common Files
!C:=C:\msys64
SHELL=/usr/bin/bash
NUMBER_OF_PROCESSORS=8
FPS_BROWSER_USER_PROFILE_STRING=Default
PROCESSOR_LEVEL=6
WD=C:\msys64\usr\bin\
TERM_PROGRAM_VERSION=3.6.3
MINGW_PREFIX=/mingw64
ERLANG_HOME=C:\Program Files\erl9.2
PKG_CONFIG_PATH=/mingw64/lib/pkgconfig:/mingw64/share/pkgconfig
USERDOMAIN_ROAMINGPROFILE=DESKTOP-JQOE2UL
GRAIL=/c/msys64/home/Juan Jimenez/GrailGUI
HOSTNAME=DESKTOP-JQOE2UL
PROGRAMFILES=C:\Program Files
MSYSTEM=MINGW64
ChocolateyInstall=C:\ProgramData\chocolatey
PATHEXT=.COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC;.PY;.PYW
NIEXTCCOMPILERSUPP=C:\Program Files (x86)\National Instruments\Shared\ExternalCompilerSupport\C\
ORIGINAL_TEMP=/c/Users/17326/AppData/Local/Temp
MINGW_CHOST=x86_64-w64-mingw32
OS=Windows_NT
HOMEDRIVE=C:
VXIPNPPATH=C:\Program Files (x86)\IVI Foundation\VISA\
RABBITMQ_NODENAME=rabbit@localhost
MSYSTEM_CARCH=x86_64
USERDOMAIN=DESKTOP-JQOE2UL
PWD=/home/Juan Jimenez
USERPROFILE=C:\Users\17326
MANPATH=/mingw64/local/man:/mingw64/share/man:/usr/local/man:/usr/share/man:/usr/man:/share/man
PRINTER=Canon TR4500 series FAX
TZ=America/New_York
MINGW_PACKAGE_PREFIX=mingw-w64-x86_64
tmp=C:\Users\17326\AppData\Local\Temp
ALLUSERSPROFILE=C:\ProgramData
ORIGINAL_PATH=/c/Windows/System32:/c/Windows:/c/Windows/System32/Wbem:/c/Windows/System32/WindowsPowerShell/v1.0/
CommonProgramW6432=C:\Program Files\Common Files
HOME=/home/Juan Jimenez
USERNAME=Juan Jimenez
NIDAQmxSwitchDir=C:\Program Files (x86)\National Instruments\NI-DAQ\Switch\
OneDrive=C:\Users\17326\OneDrive - stevens.edu
COMSPEC=C:\WINDOWS\system32\cmd.exe
APPDATA=C:\Users\17326\AppData\Roaming
SYSTEMROOT=C:\WINDOWS
LOCALAPPDATA=C:\Users\17326\AppData\Local
PROMPT=$P$G
COMPUTERNAME=DESKTOP-JQOE2UL
INFOPATH=/mingw64/local/info:/mingw64/share/info:/usr/local/info:/usr/share/info:/usr/info:/share/info
RABBITMQ_BASE=C:\ProgramData\RabbitMQ
TERM=xterm
LOGONSERVER=\\DESKTOP-JQOE2UL
ACLOCAL_PATH=/mingw64/share/aclocal:/usr/share/aclocal
USER=Juan Jimenez
PSModulePath=C:\Program Files\WindowsPowerShell\Modules;C:\WINDOWS\system32\WindowsPowerShell\v1.0\Modules;C:\Program Files (x86)\Microsoft SQL Server\120\Tools\PowerShell\Modules\
TEMP=/tmp
temp=C:\Users\17326\AppData\Local\Temp
MSYSTEM_CHOST=x86_64-w64-mingw32
ORIGINAL_TMP=/c/Users/17326/AppData/Local/Temp
SHLVL=1
PROCESSOR_REVISION=9e0a
DriverData=C:\Windows\System32\Drivers\DriverData
COMMONPROGRAMFILES=C:\Program Files\Common Files
CONICON=mingw64.ico
LC_CTYPE=en_US.UTF-8
VXIPNPPATH64=C:\Program Files\IVI Foundation\VISA\
PROCESSOR_IDENTIFIER=Intel64 Family 6 Model 158 Stepping 10, GenuineIntel
SESSIONNAME=Console
PS1=\[\e]0;\w\a\]\n\[\e[32m\]\u@\h \[\e[35m\]$MSYSTEM\[\e[0m\] \[\e[33m\]\w\[\e[0m\]\n\$
PKG_CONFIG_SYSTEM_LIBRARY_PATH=/mingw64/lib
HOMEPATH=\Users\17326
XDG_DATA_DIRS=/mingw64/share/:/usr/local/share/:/usr/share/
MSYSCON=mintty.exe
TMP=/tmp
CONFIG_SITE=/etc/config.site
PATH=/mingw64/bin:/usr/local/bin:/usr/bin:/bin:/c/Windows/System32:/c/Windows:/c/Windows/System32/Wbem:/c/Windows/System32/WindowsPowerShell/v1.0/:/usr/bin/site_perl:/usr/bin/vendor_perl:/usr/bin/core_perl:/c/msys64/home/Juan Jimenez/GrailGUI/bin
ProgramW6432=C:\Program Files
MSYSTEM_PREFIX=/mingw64
LOGINSHELL=bash
RABBITMQ_CONFIG_FILE="C:\ProgramData\National Instruments\Skyline\RabbitMQ\rabbitmq"
CONTITLE=MinGW x64
WINDIR=C:\WINDOWS
FPS_BROWSER_APP_PROFILE_STRING=Internet Explorer
PROCESSOR_ARCHITECTURE=AMD64
PUBLIC=C:\Users\Public
PKG_CONFIG_SYSTEM_INCLUDE_PATH=/mingw64/include
SYSTEMDRIVE=C:
OneDriveCommercial=C:\Users\17326\OneDrive - stevens.edu
OLDPWD=/
TERM_PROGRAM=mintty
ProgramData=C:\ProgramData
ChocolateyLastPathUpdate=132467478198832566
_=/usr/bin/env
```

env can be used for [several purposes](https://www.geeksforgeeks.org/env-command-in-linux-with-examples/) depending on arguments that are passed to it. Without arguments as seen in this example it simply prints all environment variables, although it can also be used to run a utility or command in a custom environment. 

### ps

```bash
$ ps
 PID    PPID    PGID     WINPID   TTY         UID    STIME COMMAND
 248       1     248      13668  ?         197609 10:01:47 /usr/bin/mintty
 276     249     276      11464  pty0      197609 10:19:13 /usr/bin/ps
 249     248     249      18828  pty0      197609 10:01:47 /usr/bin/bash
 238       1     238      19028  cons0     197609 18:23:56 /usr/bin/bash
```

The ps command displays all current processes, as well as their process ID and other pertinent information.
