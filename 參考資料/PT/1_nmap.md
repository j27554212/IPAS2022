#
```
nmap -sV  10.0.2.5
nmap -A  10.0.2.5   


漏洞掃描

```
## nmap掃描
```
nmap -sT -p- --min-rate 10000 -oA nmap/alltcp 192.168.4.132
nmap -sC -sV -p 21,22,80,445,631,3000,3306,3500,6697,8181 -oA nmap/services 192.168.4.132
Therefore, it might be a good idea to run some scans covering wider ranges of ports:

nmap -sV --osscan-guess -p 1-10000 [IP Address]
nmap -T4 -sV --version-all --osscan-guess -A -p 1-10000 [IP Address]
nmap -T4 -PA -sV --version-all --osscan-guess -A -p 1-10000 [IP Address]
nmap -T4 -PA -sC -sV --version-all --osscan-guess -A -p 1-10000 [IP Address]
nmap -T4 -PA -sC -sV --version-all --osscan-guess -A -p 1-65535 [IP Address]

and even UDP ports:

nmap -sU -sV --version-all -p 1-10000 [IP Address]
```
## sudo nmap -sV 10.0.2.5
```
sudo nmap -sV 10.0.2.5
Starting Nmap 7.91 ( https://nmap.org ) at 2021-12-06 04:38 EST
Nmap scan report for 10.0.2.5
Host is up (0.00077s latency).
Not shown: 989 filtered ports
PORT      STATE SERVICE  VERSION
21/tcp    open  ftp      Microsoft ftpd
22/tcp    open  ssh      OpenSSH 7.1 (protocol 2.0)
80/tcp    open  http     Microsoft IIS httpd 7.5
3000/tcp  open  http     WEBrick httpd 1.3.1 (Ruby 2.3.1 (2016-04-26))
4848/tcp  open  ssl/http Oracle Glassfish Application Server
8022/tcp  open  http     Apache Tomcat/Coyote JSP engine 1.1
8080/tcp  open  http     Sun GlassFish Open Source Edition  4.0
9200/tcp  open  wap-wsp?
49153/tcp open  msrpc    Microsoft Windows RPC
49154/tcp open  msrpc    Microsoft Windows RPC
49167/tcp open  java-rmi Java RMI
1 service unrecognized despite returning data. 

If you know the service/version, please submit the following fingerprint at https://nmap.org/cgi-bin/submit.cgi?new-service :
SF-Port9200-TCP:V=7.91%I=7%D=12/6%Time=61ADDA21%P=x86_64-pc-linux-gnu%r(Ge
SF:tRequest,191,"HTTP/1\.0\x20200\x20OK\r\nContent-Type:\x20application/js
SF:on;\x20charset=UTF-8\r\nContent-Length:\x20314\r\n\r\n{\r\n\x20\x20\"st
SF:atus\"\x20:\x20200,\r\n\x20\x20\"name\"\x20:\x20\"Douglas\x20Ramsey\",\
SF:r\n\x20\x20\"version\"\x20:\x20{\r\n\x20\x20\x20\x20\"number\"\x20:\x20
SF:\"1\.1\.1\",\r\n\x20\x20\x20\x20\"build_hash\"\x20:\x20\"f1585f096d3f39
SF:85e73456debdc1a0745f512bbc\",\r\n\x20\x20\x20\x20\"build_timestamp\"\x2
SF:0:\x20\"2014-04-16T14:27:12Z\",\r\n\x20\x20\x20\x20\"build_snapshot\"\x
SF:20:\x20false,\r\n\x20\x20\x20\x20\"lucene_version\"\x20:\x20\"4\.7\"\r\
SF:n\x20\x20},\r\n\x20\x20\"tagline\"\x20:\x20\"You\x20Know,\x20for\x20Sea
SF:rch\"\r\n}\n")%r(HTTPOptions,4F,"HTTP/1\.0\x20200\x20OK\r\nContent-Type
SF::\x20text/plain;\x20charset=UTF-8\r\nContent-Length:\x200\r\n\r\n")%r(R
SF:TSPRequest,4F,"HTTP/1\.1\x20200\x20OK\r\nContent-Type:\x20text/plain;\x
SF:20charset=UTF-8\r\nContent-Length:\x200\r\n\r\n")%r(FourOhFourRequest,A
SF:9,"HTTP/1\.0\x20400\x20Bad\x20Request\r\nContent-Type:\x20text/plain;\x
SF:20charset=UTF-8\r\nContent-Length:\x2080\r\n\r\nNo\x20handler\x20found\
SF:x20for\x20uri\x20\[/nice%20ports%2C/Tri%6Eity\.txt%2ebak\]\x20and\x20me
SF:thod\x20\[GET\]")%r(SIPOptions,4F,"HTTP/1\.1\x20200\x20OK\r\nContent-Ty
SF:pe:\x20text/plain;\x20charset=UTF-8\r\nContent-Length:\x200\r\n\r\n");
MAC Address: 08:00:27:E7:49:C5 (Oracle VirtualBox virtual NIC)
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows

Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
Nmap done: 1 IP address (1 host up) scanned in 133.26 seconds
```


## nmap -A  10.0.2.5
```
nmap -A  10.0.2.5                                                                                                      1 ⚙
Starting Nmap 7.91 ( https://nmap.org ) at 2021-12-07 06:22 EST
Nmap scan report for 10.0.2.5
Host is up (0.0032s latency).
Not shown: 978 closed ports
PORT      STATE SERVICE              VERSION
21/tcp    open  ftp                  Microsoft ftpd
| ftp-syst: 
|_  SYST: Windows_NT
22/tcp    open  ssh                  OpenSSH 7.1 (protocol 2.0)
| ssh-hostkey: 
|   2048 fb:d4:9f:b7:db:cc:91:e6:55:71:88:1e:ba:68:c7:78 (RSA)
|_  521 dc:3e:0c:bf:00:13:de:d4:28:36:cf:0c:c5:26:59:34 (ECDSA)
80/tcp    open  http                 Microsoft IIS httpd 7.5
| http-methods: 
|_  Potentially risky methods: TRACE
|_http-server-header: Microsoft-IIS/7.5
|_http-title: Site doesn't have a title (text/html).
135/tcp   open  msrpc                Microsoft Windows RPC
139/tcp   open  netbios-ssn          Microsoft Windows netbios-ssn
445/tcp   open  microsoft-ds         Windows Server 2008 R2 Standard 7601 Service Pack 1 microsoft-ds
3000/tcp  open  http                 WEBrick httpd 1.3.1 (Ruby 2.3.1 (2016-04-26))
|_http-server-header: WEBrick/1.3.1 (Ruby/2.3.1/2016-04-26)
|_http-title: Ruby on Rails: Welcome aboard
3306/tcp  open  mysql                MySQL 5.5.20-log
| mysql-info: 
|   Protocol: 10
|   Version: 5.5.20-log
|   Thread ID: 8
|   Capabilities flags: 63487
|   Some Capabilities: LongColumnFlag, InteractiveClient, Speaks41ProtocolNew, IgnoreSpaceBeforeParenthesis, SupportsTransactions, IgnoreSigpipes, Support41Auth, ConnectWithDatabase, SupportsLoadDataLocal, FoundRows, Speaks41ProtocolOld, ODBCClient, LongPassword, DontAllowDatabaseTableColumn, SupportsCompression, SupportsMultipleStatments, SupportsMultipleResults, SupportsAuthPlugins
|   Status: Autocommit
|   Salt: jzF/VE5x}-e7#GzTq_e_
|_  Auth Plugin Name: mysql_native_password
3389/tcp  open  ssl/ms-wbt-server?
| rdp-ntlm-info: 
|   Target_Name: METASPLOITABLE3
|   NetBIOS_Domain_Name: METASPLOITABLE3
|   NetBIOS_Computer_Name: METASPLOITABLE3
|   DNS_Domain_Name: metasploitable3
|   DNS_Computer_Name: metasploitable3
|   Product_Version: 6.1.7601
|_  System_Time: 2021-12-07T11:24:27+00:00
| ssl-cert: Subject: commonName=metasploitable3
| Not valid before: 2021-11-08T11:52:33
|_Not valid after:  2022-05-10T11:52:33
|_ssl-date: 2021-12-07T11:24:35+00:00; +6s from scanner time.
4848/tcp  open  ssl/http             Oracle GlassFish 4.0 (Servlet 3.1; JSP 2.3; Java 1.8)
|_http-server-header: GlassFish Server Open Source Edition  4.0 
|_http-title: Login
| ssl-cert: Subject: commonName=localhost/organizationName=Oracle Corporation/stateOrProvinceName=California/countryName=US
| Not valid before: 2013-05-15T05:33:38
|_Not valid after:  2023-05-13T05:33:38
|_ssl-date: 2021-12-07T11:24:35+00:00; +6s from scanner time.
7676/tcp  open  java-message-service Java Message Service 301
8009/tcp  open  ajp13                Apache Jserv (Protocol v1.3)
|_ajp-methods: Failed to get a valid response for the OPTION request
8022/tcp  open  http                 Apache Tomcat/Coyote JSP engine 1.1
| http-methods: 
|_  Potentially risky methods: PUT DELETE
|_http-server-header: Apache-Coyote/1.1
|_http-title: Site doesn't have a title (text/html;charset=UTF-8).
8031/tcp  open  ssl/unknown
8080/tcp  open  http                 Oracle GlassFish 4.0 (Servlet 3.1; JSP 2.3; Java 1.8)
| http-methods: 
|_  Potentially risky methods: PUT DELETE TRACE
|_http-open-proxy: Proxy might be redirecting requests
|_http-server-header: GlassFish Server Open Source Edition  4.0 
|_http-title: GlassFish Server - Server Running
8181/tcp  open  ssl/http             Oracle GlassFish 4.0 (Servlet 3.1; JSP 2.3; Java 1.8)
| http-methods: 
|_  Potentially risky methods: PUT DELETE TRACE
|_http-server-header: GlassFish Server Open Source Edition  4.0 
|_http-title: Site doesn't have a title (text/html).
| ssl-cert: Subject: commonName=localhost/organizationName=Oracle Corporation/stateOrProvinceName=California/countryName=US
| Not valid before: 2013-05-15T05:33:38
|_Not valid after:  2023-05-13T05:33:38
|_ssl-date: 2021-12-07T11:24:35+00:00; +6s from scanner time.
8443/tcp  open  ssl/https-alt?
9200/tcp  open  wap-wsp?
| fingerprint-strings: 
|   FourOhFourRequest: 
|     HTTP/1.0 400 Bad Request
|     Content-Type: text/plain; charset=UTF-8
|     Content-Length: 80
|     handler found for uri [/nice%20ports%2C/Tri%6Eity.txt%2ebak] and method [GET]
|   GetRequest: 
|     HTTP/1.0 200 OK
|     Content-Type: application/json; charset=UTF-8
|     Content-Length: 307
|     "status" : 200,
|     "name" : "Phoenix",
|     "version" : {
|     "number" : "1.1.1",
|     "build_hash" : "f1585f096d3f3985e73456debdc1a0745f512bbc",
|     "build_timestamp" : "2014-04-16T14:27:12Z",
|     "build_snapshot" : false,
|     "lucene_version" : "4.7"
|     "tagline" : "You Know, for Search"
|   HTTPOptions: 
|     HTTP/1.0 200 OK
|     Content-Type: text/plain; charset=UTF-8
|     Content-Length: 0
|   RTSPRequest, SIPOptions: 
|     HTTP/1.1 200 OK
|     Content-Type: text/plain; charset=UTF-8
|_    Content-Length: 0
49152/tcp open  msrpc                Microsoft Windows RPC
49153/tcp open  msrpc                Microsoft Windows RPC
49154/tcp open  msrpc                Microsoft Windows RPC
49156/tcp open  msrpc                Microsoft Windows RPC
1 service unrecognized despite returning data. If you know the service/version, please submit the following fingerprint at https://nmap.org/cgi-bin/submit.cgi?new-service :
SF-Port9200-TCP:V=7.91%I=7%D=12/7%Time=61AF43FF%P=x86_64-pc-linux-gnu%r(Ge
SF:tRequest,18A,"HTTP/1\.0\x20200\x20OK\r\nContent-Type:\x20application/js
SF:on;\x20charset=UTF-8\r\nContent-Length:\x20307\r\n\r\n{\r\n\x20\x20\"st
SF:atus\"\x20:\x20200,\r\n\x20\x20\"name\"\x20:\x20\"Phoenix\",\r\n\x20\x2
SF:0\"version\"\x20:\x20{\r\n\x20\x20\x20\x20\"number\"\x20:\x20\"1\.1\.1\
SF:",\r\n\x20\x20\x20\x20\"build_hash\"\x20:\x20\"f1585f096d3f3985e73456de
SF:bdc1a0745f512bbc\",\r\n\x20\x20\x20\x20\"build_timestamp\"\x20:\x20\"20
SF:14-04-16T14:27:12Z\",\r\n\x20\x20\x20\x20\"build_snapshot\"\x20:\x20fal
SF:se,\r\n\x20\x20\x20\x20\"lucene_version\"\x20:\x20\"4\.7\"\r\n\x20\x20}
SF:,\r\n\x20\x20\"tagline\"\x20:\x20\"You\x20Know,\x20for\x20Search\"\r\n}
SF:\n")%r(HTTPOptions,4F,"HTTP/1\.0\x20200\x20OK\r\nContent-Type:\x20text/
SF:plain;\x20charset=UTF-8\r\nContent-Length:\x200\r\n\r\n")%r(RTSPRequest
SF:,4F,"HTTP/1\.1\x20200\x20OK\r\nContent-Type:\x20text/plain;\x20charset=
SF:UTF-8\r\nContent-Length:\x200\r\n\r\n")%r(FourOhFourRequest,A9,"HTTP/1\
SF:.0\x20400\x20Bad\x20Request\r\nContent-Type:\x20text/plain;\x20charset=
SF:UTF-8\r\nContent-Length:\x2080\r\n\r\nNo\x20handler\x20found\x20for\x20
SF:uri\x20\[/nice%20ports%2C/Tri%6Eity\.txt%2ebak\]\x20and\x20method\x20\[
SF:GET\]")%r(SIPOptions,4F,"HTTP/1\.1\x20200\x20OK\r\nContent-Type:\x20tex
SF:t/plain;\x20charset=UTF-8\r\nContent-Length:\x200\r\n\r\n");
Service Info: OSs: Windows, Windows Server 2008 R2 - 2012; CPE: cpe:/o:microsoft:windows

Host script results:
|_clock-skew: mean: 1h08m40s, deviation: 3h01m25s, median: 5s
|_nbstat: NetBIOS name: METASPLOITABLE3, NetBIOS user: <unknown>, NetBIOS MAC: 08:00:27:e7:49:c5 (Oracle VirtualBox virtual NIC)
| smb-os-discovery: 
|   OS: Windows Server 2008 R2 Standard 7601 Service Pack 1 (Windows Server 2008 R2 Standard 6.1)
|   OS CPE: cpe:/o:microsoft:windows_server_2008::sp1
|   Computer name: metasploitable3
|   NetBIOS computer name: METASPLOITABLE3\x00
|   Workgroup: WORKGROUP\x00
|_  System time: 2021-12-07T03:24:19-08:00
| smb-security-mode: 
|   account_used: guest
|   authentication_level: user
|   challenge_response: supported
|_  message_signing: disabled (dangerous, but default)
| smb2-security-mode: 
|   2.02: 
|_    Message signing enabled but not required
| smb2-time: 
|   date: 2021-12-07T11:24:20
|_  start_date: 2021-12-07T10:54:00

Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
Nmap done: 1 IP address (1 host up) scanned in 123.23 seconds
```

## 漏洞掃描1:掃描是否存在ms17-010的漏洞 smb-vuln-ms17-010

## 使用[NMAP nse](https://nmap.org/nsedoc/)

- 記得關閉防火牆
- netsh advfirewall set allprofiles state off
- [smb-vuln-ms17-010](https://nmap.org/nsedoc/scripts/smb-vuln-ms17-010.html)
- nmap -p445 --script smb-vuln-ms17-010 <target>

![nmap_nse_ms17-010.png](./nmap_nse_ms17-010.png)

   ## 使用[metasploit] 
```
msf6 > search ms17-010

Matching Modules
================
   #  Name                                      Disclosure Date  Rank     Check  Description
   -  ----                                      ---------------  ----     -----  -----------
   0  exploit/windows/smb/ms17_010_eternalblue  2017-03-14       average  Yes    MS17-010 EternalBlue SMB Remote Windows Kernel Pool Corruption
   1  exploit/windows/smb/ms17_010_psexec       2017-03-14       normal   Yes    MS17-010 EternalRomance/EternalSynergy/EternalChampion SMB Remote Windows Code Execution
   2  auxiliary/admin/smb/ms17_010_command      2017-03-14       normal   No     MS17-010 EternalRomance/EternalSynergy/EternalChampion SMB Remote Windows Command Execution
   3  auxiliary/scanner/smb/smb_ms17_010                         normal   No     MS17-010 SMB RCE Detection
   4  exploit/windows/smb/smb_doublepulsar_rce  2017-04-14       great    Yes    SMB DOUBLEPULSAR Remote Code Execution
Interact with a module by name or index. For example info 4, use 4 or use exploit/windows/smb/smb_doublepulsar_rce
```

```
msf6 > use auxiliary/scanner/smb/smb_ms17_010                                                                         
msf6 auxiliary(scanner/smb/smb_ms17_010) > show options                                                               
                                                                                                                      
Module options (auxiliary/scanner/smb/smb_ms17_010):                                                                  
                                                                                                                      
   Name         Current Setting                     Required  Description                                             
   ----         ---------------                     --------  -----------                                             
   CHECK_ARCH   true                                no        Check for architecture on vulnerable hosts                     
   CHECK_DOPU   true                                no        Check for DOUBLEPULSAR on vulnerable hosts                     
   CHECK_PIPE   false                               no        Check for named pipe on vulnerable hosts
   NAMED_PIPES  /usr/share/metasploit-framework/da  yes       List of named pipes to check
                ta/wordlists/named_pipes.txt
   RHOSTS       10.0.2.5                            yes       The target host(s), see https://github.com/rapid7/metasploit-
                                                              framework/wiki/Using-Metasploit
   RPORT        445                                 yes       The SMB service port (TCP)
   SMBDomain    .                                   no        The Windows domain to use for authentication
   SMBPass                                          no        The password for the specified username
   SMBUser                                          no        The username to authenticate as
   THREADS      1                                   yes       The number of concurrent threads (max one per host)

msf6 auxiliary(scanner/smb/smb_ms17_010) > exploit
[+] 10.0.2.5:445          - Host is likely VULNERABLE to MS17-010! - Windows Server 2008 R2 Standard 7601 Service Pack 1 x64 (64-bit)
[*] 10.0.2.5:445          - Scanned 1 of 1 hosts (100% complete)
[*] Auxiliary module execution completed
```
