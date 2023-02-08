# Lab 2 - Raspberry Pi and Command Shell

## Lab Commands: Execution and Output

As part of the lab we are going to execute some terminal commands, display their output on my local machine, and we are going to define their function based on these outputs:

### **hostname**

```bash
$ hostname
DESKTOP-JQOE2UL
```

This command displays the current host, domain, or node name of the system. It uniquely identifies a computer in a network.

### **env**

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

### **ps**

```bash
$ ps
 PID    PPID    PGID     WINPID   TTY         UID    STIME COMMAND
 248       1     248      13668  ?         197609 10:01:47 /usr/bin/mintty
 276     249     276      11464  pty0      197609 10:19:13 /usr/bin/ps
 249     248     249      18828  pty0      197609 10:01:47 /usr/bin/bash
 238       1     238      19028  cons0     197609 18:23:56 /usr/bin/bash
```

The ps command displays all current processes, as well as their process ID and other pertinent information.

### **pwd**

```bash
$ pwd
/home/Juan Jimenez
```

The pwd command displays the output of the full path name of your current directory (from the root directory).

### **git clone [repository_address]**

```bash
$ git clone https://github.com/kevinwlu/iot.git
Cloning into 'iot'...
remote: Enumerating objects: 17490, done.
remote: Counting objects: 100% (204/204), done.
remote: Compressing objects: 100% (86/86), done.
remote: Total 17490 (delta 92), reused 174 (delta 80), pack-reused 17286
Receiving objects: 100% (17490/17490), 27.37 MiB | 26.44 MiB/s, done.
Resolving deltas: 100% (11823/11823), done.
Updating files: 100% (388/388), done.
```

The git clone command downloads a remote repository from GitHub to your local machine. Uses SSH keys for verification.

### **cd [directory_name]**

```bash
cd iot
```

The cd command is used to change current working directories. It is used to navigate directories by indicating the name of the directory you would like to navigate to after typing cd.

### **ls**

```bash
$ ls
README.md  economics  lesson10  lesson4  lesson7  projects          tools
apps       hype       lesson2   lesson5  lesson8  special_problems
cases      lesson1    lesson3   lesson6  lesson9  standards
```

The ls commands lists all files and directories in the current working directory.

### **cd**

```bash
$ cd
Juan Jimenez@DESKTOP-JQOE2UL MINGW64 ~
```

The cd command without any arugments returns you to the root directory. 

### **df**

```bash
$ df
Filesystem     1K-blocks      Used Available Use% Mounted on
C:/msys64      431958296 333458152  98500144  78% /
```

The df command displays the amount of disk space available on the filesystem with each file name's argument.

### **mkdir [directory_name]**

```bash
mkdir demo
cd demo
```

creates a directory in the current working directory with the given argument name. cd is used to navigate to the newly created directory.

### **nano [file_name]**

```bash
nano file
```

Creates a new text file using [nano](https://www.nano-editor.org/) and opens the file to be edited using the nano application.

### **cat [file_name]**

```bash
$ cat file
hello world
```

The cat command prints the content of a file onto the stantard output stream. 

### **cp [file] [new_file]**

```bash
cp file file1

```

The cp command copies the contents from one file into another file. In this case it copies the contents of one file into a new file with a different name.

### **mv [file] [new_file_name]**

```bash
mv file file2

```

The mv command moves files and directories from one directory to another or renames a file or directory. In this case file was renamed to file2.

### **rm [file_name]**

```bash
rm file2

```

The rm command deletes files from the directory by the given argument name.

### **clear**

```bash
clear

```

The clear command removes all previous commands from the output of the terminal and refresh the temrinal to give the appearance of a newly opened terminal. 

### **man [command_name]**

```bash
man uname

```

The man command in Linux is used to display the user manual of any command that we can run on the terminal. In this case uname is used to print system information.

### **uname -a**

```bash
$ uname -a
MINGW64_NT-10.0-19044 DESKTOP-JQOE2UL 3.4.5.x86_64 2023-01-20 09:17 UTC x86_64 Msys
```

The command uname -a prints out all relevant system information.

### **ifconfig**

```bash
 $ ifconfig
eth0: flags=4099<UP,BROADCAST,MULTICAST>  mtu 1500
        ether e4:5f:01:79:51:11  txqueuelen 1000  (Ethernet)
        RX packets 0  bytes 0 (0.0 B)
        RX errors 0  dropped 0  overruns 0  frame 0
        TX packets 0  bytes 0 (0.0 B)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0

lo: flags=73<UP,LOOPBACK,RUNNING>  mtu 65536
        inet 127.0.0.1  netmask 255.0.0.0
        inet6 ::1  prefixlen 128  scopeid 0x10<host>
        loop  txqueuelen 1000  (Local Loopback)
        RX packets 216  bytes 19534 (19.0 KiB)
        RX errors 0  dropped 0  overruns 0  frame 0
        TX packets 216  bytes 19534 (19.0 KiB)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0

wlan0: flags=4163<UP,BROADCAST,RUNNING,MULTICAST>  mtu 1500
        inet 192.168.1.179  netmask 255.255.255.0  broadcast 192.168.1.255
        inet6 2600:4041:41d1:c200:64cb:13a6:a5f5:a5ee  prefixlen 64  scopeid 0x0<global>
        inet6 fe80::8bc3:c896:b971:5b54  prefixlen 64  scopeid 0x20<link>
        ether e4:5f:01:79:51:12  txqueuelen 1000  (Ethernet)
        RX packets 129  bytes 12317 (12.0 KiB)
        RX errors 0  dropped 0  overruns 0  frame 0
        TX packets 168  bytes 21514 (21.0 KiB)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0
```

The ifconfig command stand for network interface configuration, without any arguments it displays the current functioning network interfaces as well as data pertaining to them. 

### **ping [host_name]**

```bash
$ ping localhost

Pinging DESKTOP-JQOE2UL [::1] with 32 bytes of data:
Reply from ::1: time<1ms
Reply from ::1: time<1ms
Reply from ::1: time<1ms
Reply from ::1: time<1ms

Ping statistics for ::1:
    Packets: Sent = 4, Received = 4, Lost = 0 (0% loss),
Approximate round trip times in milli-seconds:
    Minimum = 0ms, Maximum = 0ms, Average = 0m
```

The ping command sends a message to the host that is desired. It can be used to test if a server is up and executing.

### **netstat**

```bash
$ netstat

Active Connections

  Proto  Local Address          Foreign Address        State
  TCP    127.0.0.1:4369         checkhost:49803        ESTABLISHED
  TCP    127.0.0.1:4369         checkhost:61341        TIME_WAIT
  TCP    127.0.0.1:4369         checkhost:61353        TIME_WAIT
  TCP    127.0.0.1:49673        checkhost:49674        ESTABLISHED
  TCP    127.0.0.1:49674        checkhost:49673        ESTABLISHED
  TCP    127.0.0.1:49679        checkhost:49680        ESTABLISHED
  TCP    127.0.0.1:49680        checkhost:49679        ESTABLISHED
  TCP    127.0.0.1:49681        checkhost:61900        ESTABLISHED
  TCP    127.0.0.1:49682        checkhost:49683        ESTABLISHED
  TCP    127.0.0.1:49683        checkhost:49682        ESTABLISHED
  TCP    127.0.0.1:49684        checkhost:49782        ESTABLISHED
  TCP    127.0.0.1:49685        checkhost:49686        ESTABLISHED
  TCP    127.0.0.1:49686        checkhost:49685        ESTABLISHED
  TCP    127.0.0.1:49691        checkhost:49846        ESTABLISHED
  TCP    127.0.0.1:49700        checkhost:49701        ESTABLISHED
  TCP    127.0.0.1:49701        checkhost:49700        ESTABLISHED
  TCP    127.0.0.1:49702        checkhost:61900        ESTABLISHED
  TCP    127.0.0.1:49703        checkhost:49704        ESTABLISHED
  TCP    127.0.0.1:49704        checkhost:49703        ESTABLISHED
  TCP    127.0.0.1:49709        checkhost:49721        ESTABLISHED
  TCP    127.0.0.1:49709        checkhost:49723        ESTABLISHED
  TCP    127.0.0.1:49709        checkhost:49725        ESTABLISHED
  TCP    127.0.0.1:49709        checkhost:49728        ESTABLISHED
  TCP    127.0.0.1:49709        checkhost:49729        ESTABLISHED
  TCP    127.0.0.1:49709        checkhost:49732        ESTABLISHED
  TCP    127.0.0.1:49709        checkhost:49737        ESTABLISHED
  TCP    127.0.0.1:49709        checkhost:49754        ESTABLISHED
  TCP    127.0.0.1:49712        checkhost:49713        ESTABLISHED
  TCP    127.0.0.1:49713        checkhost:49712        ESTABLISHED
  TCP    127.0.0.1:49714        checkhost:61900        ESTABLISHED
  TCP    127.0.0.1:49715        checkhost:49716        ESTABLISHED
  TCP    127.0.0.1:49716        checkhost:49715        ESTABLISHED
  TCP    127.0.0.1:49721        checkhost:49709        ESTABLISHED
  TCP    127.0.0.1:49723        checkhost:49709        ESTABLISHED
  TCP    127.0.0.1:49725        checkhost:49709        ESTABLISHED
  TCP    127.0.0.1:49728        checkhost:49709        ESTABLISHED
  TCP    127.0.0.1:49729        checkhost:49709        ESTABLISHED
  TCP    127.0.0.1:49732        checkhost:49709        ESTABLISHED
  TCP    127.0.0.1:49737        checkhost:49709        ESTABLISHED
  TCP    127.0.0.1:49741        checkhost:49742        ESTABLISHED
  TCP    127.0.0.1:49742        checkhost:49741        ESTABLISHED
  TCP    127.0.0.1:49743        checkhost:61900        ESTABLISHED
  TCP    127.0.0.1:49744        checkhost:49745        ESTABLISHED
  TCP    127.0.0.1:49745        checkhost:49744        ESTABLISHED
  TCP    127.0.0.1:49754        checkhost:49709        ESTABLISHED
  TCP    127.0.0.1:49756        checkhost:49757        ESTABLISHED
  TCP    127.0.0.1:49757        checkhost:49756        ESTABLISHED
  TCP    127.0.0.1:49776        checkhost:49777        ESTABLISHED
  TCP    127.0.0.1:49777        checkhost:49776        ESTABLISHED
  TCP    127.0.0.1:49780        checkhost:49781        ESTABLISHED
  TCP    127.0.0.1:49781        checkhost:49780        ESTABLISHED
  TCP    127.0.0.1:49782        checkhost:49684        ESTABLISHED
  TCP    127.0.0.1:49783        checkhost:49784        ESTABLISHED
  TCP    127.0.0.1:49784        checkhost:49783        ESTABLISHED
  TCP    127.0.0.1:49792        checkhost:49793        ESTABLISHED
  TCP    127.0.0.1:49793        checkhost:49792        ESTABLISHED
  TCP    127.0.0.1:49803        checkhost:4369         ESTABLISHED
  TCP    127.0.0.1:49846        checkhost:49691        ESTABLISHED
  TCP    127.0.0.1:49851        checkhost:49852        ESTABLISHED
  TCP    127.0.0.1:49852        checkhost:49851        ESTABLISHED
  TCP    127.0.0.1:49868        checkhost:65001        ESTABLISHED
  TCP    127.0.0.1:49873        checkhost:60096        ESTABLISHED
  TCP    127.0.0.1:60096        checkhost:49873        ESTABLISHED
  TCP    127.0.0.1:61900        checkhost:49681        ESTABLISHED
  TCP    127.0.0.1:61900        checkhost:49702        ESTABLISHED
  TCP    127.0.0.1:61900        checkhost:49714        ESTABLISHED
  TCP    127.0.0.1:61900        checkhost:49743        ESTABLISHED
  TCP    127.0.0.1:65001        checkhost:49868        ESTABLISHED
  TCP    192.168.1.173:49425    52.159.126.152:https   ESTABLISHED
  TCP    192.168.1.173:58298    52.159.127.243:https   ESTABLISHED
  TCP    192.168.1.173:60105    13.73.252.131:8883     ESTABLISHED
  TCP    192.168.1.173:60188    ec2-3-209-45-201:https  TIME_WAIT
  TCP    192.168.1.173:60193    104.36.115.111:https   TIME_WAIT
  TCP    192.168.1.173:60195    server-18-161-39-198:https  TIME_WAIT
  TCP    192.168.1.173:60202    ec2-54-81-181-65:https  TIME_WAIT
  TCP    192.168.1.173:60271    ec2-52-6-125-14:https  TIME_WAIT
  TCP    192.168.1.173:61058    server-18-161-39-198:https  TIME_WAIT
  TCP    192.168.1.173:61188    server-108-138-128-110:https  TIME_WAIT
  TCP    192.168.1.173:61202    server-18-67-65-58:https  TIME_WAIT
  TCP    192.168.1.173:61210    a12b7a488abeaa9e4:https  TIME_WAIT
  TCP    192.168.1.173:61213    ec2-3-219-55-168:https  TIME_WAIT
  TCP    192.168.1.173:61219    104.18.20.134:https    TIME_WAIT
  TCP    192.168.1.173:61221    ec2-52-72-127-126:https  TIME_WAIT
  TCP    192.168.1.173:61225    ec2-52-204-114-10:https  TIME_WAIT
  TCP    192.168.1.173:61232    server-108-138-115-22:https  TIME_WAIT
  TCP    192.168.1.173:61233    server-18-161-21-43:https  TIME_WAIT
  TCP    192.168.1.173:61236    194:https              TIME_WAIT
  TCP    192.168.1.173:61270    lga34s35-in-f5:https   TIME_WAIT
  TCP    192.168.1.173:61289    51.104.167.255:https   TIME_WAIT
  TCP    192.168.1.173:61297    lb-140-82-114-3-iad:https  TIME_WAIT
  TCP    192.168.1.173:61346    102:https              TIME_WAIT
  TCP    192.168.1.173:61347    102:https              TIME_WAIT
  TCP    [::1]:49675            DESKTOP-JQOE2UL:49676  ESTABLISHED
  TCP    [::1]:49676            DESKTOP-JQOE2UL:49675  ESTABLISHED
  TCP    [::1]:49677            DESKTOP-JQOE2UL:49678  ESTABLISHED
  TCP    [::1]:49678            DESKTOP-JQOE2UL:49677  ESTABLISHED
  TCP    [::1]:49689            DESKTOP-JQOE2UL:49690  ESTABLISHED
  TCP    [::1]:49690            DESKTOP-JQOE2UL:49689  ESTABLISHED
  TCP    [::1]:49705            DESKTOP-JQOE2UL:49706  ESTABLISHED
  TCP    [::1]:49706            DESKTOP-JQOE2UL:49705  ESTABLISHED
  TCP    [2600:4041:41d1:c200:4d2:4d15:6614:e699]:60118  [2603:1036:302:4831::2]:https  TIME_WAIT
  TCP    [2600:4041:41d1:c200:4d2:4d15:6614:e699]:60238  lga25s71-in-x0a:https  TIME_WAIT
  TCP    [2600:4041:41d1:c200:4d2:4d15:6614:e699]:60268  [2606:4700:20::ac43:4686]:https  TIME_WAIT
  TCP    [2600:4041:41d1:c200:4d2:4d15:6614:e699]:60394  lga15s43-in-x03:https  TIME_WAIT
  TCP    [2600:4041:41d1:c200:4d2:4d15:6614:e699]:60402  lga15s43-in-x03:https  TIME_WAIT
  TCP    [2600:4041:41d1:c200:4d2:4d15:6614:e699]:60452  lga34s34-in-x0e:https  TIME_WAIT
  TCP    [2600:4041:41d1:c200:4d2:4d15:6614:e699]:60670  [2620:1ec:bdf::254]:https  CLOSE_WAIT
  TCP    [2600:4041:41d1:c200:4d2:4d15:6614:e699]:60671  [2606:2800:11f:17a5:191a:18d5:537:22f9]:https  CLOSE_WAIT
  TCP    [2600:4041:41d1:c200:4d2:4d15:6614:e699]:61065  lga15s49-in-x02:https  TIME_WAIT
  TCP    [2600:4041:41d1:c200:4d2:4d15:6614:e699]:61117  lga34s34-in-x08:https  TIME_WAIT
  TCP    [2600:4041:41d1:c200:4d2:4d15:6614:e699]:61167  lga25s78-in-x0a:https  TIME_WAIT
  TCP    [2600:4041:41d1:c200:4d2:4d15:6614:e699]:61241  [2606:4700::6810:f9f9]:https  TIME_WAIT
  TCP    [2600:4041:41d1:c200:4d2:4d15:6614:e699]:61250  [2600:9000:25c8:1200:6:8656:f5c0:93a1]:https  TIME_WAIT
  TCP    [2600:4041:41d1:c200:4d2:4d15:6614:e699]:61254  lga25s81-in-x0e:https  TIME_WAIT
  TCP    [2600:4041:41d1:c200:4d2:4d15:6614:e699]:61259  lga25s73-in-x02:https  TIME_WAIT
  TCP    [2600:4041:41d1:c200:4d2:4d15:6614:e699]:61260  lga34s32-in-x02:https  TIME_WAIT
  TCP    [2600:4041:41d1:c200:4d2:4d15:6614:e699]:61271  lga34s38-in-x04:https  TIME_WAIT
  TCP    [2600:4041:41d1:c200:4d2:4d15:6614:e699]:61272  lga34s38-in-x04:https  TIME_WAIT
  TCP    [2600:4041:41d1:c200:4d2:4d15:6614:e699]:61275  lga34s37-in-x05:https  TIME_WAIT
  TCP    [2600:4041:41d1:c200:4d2:4d15:6614:e699]:61276  lga34s37-in-x05:https  TIME_WAIT
  TCP    [2600:4041:41d1:c200:4d2:4d15:6614:e699]:61277  lga34s37-in-x0a:https  TIME_WAIT
  TCP    [2600:4041:41d1:c200:4d2:4d15:6614:e699]:61278  lga34s37-in-x0a:https  TIME_WAIT
  TCP    [2600:4041:41d1:c200:4d2:4d15:6614:e699]:61307  lga25s73-in-x02:https  TIME_WAIT
  TCP    [2600:4041:41d1:c200:4d2:4d15:6614:e699]:61316  lga34s35-in-x02:https  TIME_WAIT
  TCP    [2600:4041:41d1:c200:4d2:4d15:6614:e699]:61317  lga34s35-in-x02:https  TIME_WAIT
  TCP    [2600:4041:41d1:c200:4d2:4d15:6614:e699]:61328  lga25s81-in-x04:https  TIME_WAIT
  TCP    [2600:4041:41d1:c200:4d2:4d15:6614:e699]:61330  lga25s73-in-x02:https  TIME_WAIT
  TCP    [2600:4041:41d1:c200:4d2:4d15:6614:e699]:61331  lga25s73-in-x02:https  TIME_WAIT
  TCP    [2600:4041:41d1:c200:4d2:4d15:6614:e699]:61349  [2600:1901:0:e988::]:https  TIME_WAIT
  TCP    [2600:4041:41d1:c200:4d2:4d15:6614:e699]:61350  [2600:1901:0:e988::]:https  TIME_WAIT
  TCP    [2600:4041:41d1:c200:4d2:4d15:6614:e699]:61351  lga34s33-in-x0a:https  TIME_WAIT
  TCP    [2600:4041:41d1:c200:4d2:4d15:6614:e699]:61354  lga15s43-in-x0e:https  TIME_WAIT
  TCP    [2600:4041:41d1:c200:4d2:4d15:6614:e699]:61357  lga34s33-in-x0e:https  TIME_WAIT
```

The netstat command prints out all connected devices to the host.
