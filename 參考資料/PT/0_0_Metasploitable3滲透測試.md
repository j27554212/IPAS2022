# Metasploitable 3


## 教學影片
- [Windows Penetration Testing Training - Metasploitable 3](https://www.youtube.com/watch?v=_ztZ_es9FT4)
- [Learning Metasploitable 3 Part 2 - Windows Penetration Testing and Cybersecurity Training](https://www.youtube.com/watch?v=kVE5rXfFbe8)
## 教學文件
- [Metasploitable3 - Exploiting UnrealIRC Service](https://ricobandy.github.io/metasploitable3/metasploitable-3-irc/)
- [Metasploitable 3 渗透测试实战](https://www.codenong.com/js7816bec59861/)
- [Metasploitable 3 实战渗透测试](https://www.codenong.com/js7816bec59861/)
- [Windows系统安全3——渗透利器](https://blog.csdn.net/m0_55401536/article/details/120253909)
- [Metasploitable 3 Windows Walkthrough: Part I](https://tremblinguterus.blogspot.com/2020/11/metasploitable-3-windows-walkthrough_34.html)
- [Metasploitable 3 实战渗透测试](https://blog.csdn.net/weixin_51167520/article/details/114745286?spm=1001.2101.3001.6661.1&utm_medium=distribute.pc_relevant_t0.none-task-blog-2%7Edefault%7ECTRLIST%7Edefault-1.opensearchhbase&depth_1-utm_source=distribute.pc_relevant_t0.none-task-blog-2%7Edefault%7ECTRLIST%7Edefault-1.opensearchhbase)
## 系統測試架構

## Metasploitable 3
- windows 2008
- 內置一些安全機制，比如防火牆，許可權設置等
- 也可以建置在linux, see [Metasploitable3 - Building the Ubuntu Linux Version](https://www.thomaslaurenson.com/blog/2018-07-08/metasploitable3-pentesting-the-ubuntu-linux-version-part1/)
- Username: vagrant Password: vagrant
- Check  PowerShell Version  
  - (Get-Host).Version
  - $host.Version
  - $PSVersionTable.PSVersion
  - (Get-ItemProperty -Path HKLM:\SOFTWARE\Microsoft\PowerShell\3\PowerShellEngine -Name 'PowerShellVersion').PowerShellVersion
- [Metasploitable 3有哪些漏洞?](https://github.com/rapid7/metasploitable3/wiki/Vulnerabilities)

- 記得關閉防火牆
- netsh advfirewall set allprofiles state off

## Kali linux



## 進入metasploit Kali-2021.3
- 進入metasploit ==> msfconsole
```
       =[ metasploit v6.1.4-dev                           ]
+ -- --=[ 2162 exploits - 1147 auxiliary - 367 post       ]
+ -- --=[ 592 payloads - 45 encoders - 10 nops            ]
+ -- --=[ 8 evasion                                       ]
```
## MS17-010 攻擊
```
掃描是否存在ms17-010的漏洞
搜尋ms17-010的攻擊碼
執行ms17-010的攻擊
post-exploitation 
```
### [掃描是否存在ms17-010的漏洞 smb-vuln-ms17-010](https://nmap.org/nsedoc/scripts/smb-vuln-ms17-010.html)

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
## [SSH暴力攻擊](https://officeguide.cc/metasploit-penetration-testing-framework-metasploitable-tutorial-examples/)
```
search 指令搜尋 ssh 相關的模組 ==> search ssh
偵測 SSH 伺服器版本的模組，並查看該模組的相關參數 ==> 
```
- 對 SSH 的 22 連接埠進行暴力攻擊 

- search 指令搜尋 ssh 相關的模組 ==> search ssh
```
msf6 > search ssh -wide

Matching Modules
================

   #   Name                                                        Disclosure Date  Rank       Check  Description
   -   ----                                                        ---------------  ----       -----  -----------
   0   exploit/linux/http/alienvault_exec                          2017-01-31       excellent  Yes    AlienVault OSSIM/USM Remote Code Execution
   1   auxiliary/scanner/ssh/apache_karaf_command_execution        2016-02-09       normal     No     Apache Karaf Default Credentials Command Execution
   2   auxiliary/scanner/ssh/karaf_login                                            normal     No     Apache Karaf Login Utility
   3   exploit/apple_ios/ssh/cydia_default_ssh                     2007-07-02       excellent  No     Apple iOS Default SSH Password Vulnerability
   4   exploit/unix/ssh/arista_tacplus_shell                       2020-02-02       great      Yes    Arista restricted shell escape (with privesc)
   5   exploit/unix/ssh/array_vxag_vapv_privkey_privesc            2014-02-03       excellent  No     Array Networks vAPV and vxAG Private Key Privilege Escalation Code Execution
   6   exploit/linux/ssh/ceragon_fibeair_known_privkey             2015-04-01       excellent  No     Ceragon FibeAir IP-10 SSH Private Key Exposure
   7   auxiliary/scanner/ssh/cerberus_sftp_enumusers               2014-05-27       normal     No     Cerberus FTP Server SFTP Username Enumeration
   8   auxiliary/dos/cisco/cisco_7937g_dos                         2020-06-02       normal     No     Cisco 7937G Denial-of-Service Attack
   9   auxiliary/admin/http/cisco_7937g_ssh_privesc                2020-06-02       normal     No     Cisco 7937G SSH Privilege Escalation
   10  auxiliary/scanner/http/cisco_firepower_login                                 normal     No     Cisco Firepower Management Console 6.0 Login
   11  exploit/linux/ssh/cisco_ucs_scpuser                         2019-08-21       excellent  No     Cisco UCS Director default scpuser password
   12  auxiliary/scanner/ssh/eaton_xpert_backdoor                  2018-07-18       normal     No     Eaton Xpert Meter SSH Private Key Exposure Scanner
   13  exploit/linux/ssh/exagrid_known_privkey                     2016-04-07       excellent  No     ExaGrid Known SSH Key and Default Password
   14  exploit/linux/ssh/f5_bigip_known_privkey                    2012-06-11       excellent  No     F5 BIG-IP SSH Private Key Exposure
   15  auxiliary/scanner/ssh/fortinet_backdoor                     2016-01-09       normal     No     Fortinet SSH Backdoor Scanner
   16  post/windows/manage/forward_pageant                                          normal     No     Forward SSH Agent Requests To Remote Pageant
   17  exploit/windows/ssh/freeftpd_key_exchange                   2006-05-12       average    No     FreeFTPd 1.0.10 Key Exchange Algorithm String Buffer Overflow
   18  exploit/windows/ssh/freesshd_key_exchange                   2006-05-12       average    No     FreeSSHd 1.0.9 Key Exchange Algorithm String Buffer Overflow
   19  exploit/windows/ssh/freesshd_authbypass                     2010-08-11       excellent  Yes    Freesshd Authentication Bypass
   20  auxiliary/scanner/http/gitlab_user_enum                     2014-11-21       normal     No     GitLab User Enumeration
   21  exploit/multi/http/gitlab_shell_exec                        2013-11-04       excellent  Yes    Gitlab-shell Code Execution
   22  exploit/linux/ssh/ibm_drm_a3user                            2020-04-21       excellent  No     IBM Data Risk Manager a3user Default Password
   23  post/windows/manage/install_ssh                                              normal     No     Install OpenSSH for Windows
   24  post/multi/gather/jenkins_gather                                             normal     No     Jenkins Credential Collector
   25  auxiliary/scanner/ssh/juniper_backdoor                      2015-12-20       normal     No     Juniper SSH Backdoor Scanner
   26  auxiliary/scanner/ssh/detect_kippo                                           normal     No     Kippo SSH Honeypot Detector
   27  post/linux/gather/enum_network                                               normal     No     Linux Gather Network Information
   28  exploit/linux/local/ptrace_traceme_pkexec_helper            2019-07-04       excellent  Yes    Linux Polkit pkexec helper PTRACE_TRACEME local root exploit
   29  exploit/linux/ssh/loadbalancerorg_enterprise_known_privkey  2014-03-17       excellent  No     Loadbalancer.org Enterprise VA SSH Private Key Exposure
   30  exploit/multi/http/git_submodule_command_exec               2017-08-10       excellent  No     Malicious Git HTTP Server For CVE-2017-1000117
   31  exploit/linux/ssh/mercurial_ssh_exec                        2017-04-18       excellent  No     Mercurial Custom hg-ssh Wrapper Remote Code Exec
   32  exploit/linux/ssh/microfocus_obr_shrboadmin                 2020-09-21       excellent  No     Micro Focus Operations Bridge Reporter shrboadmin default password
   33  post/multi/gather/ssh_creds                                                  normal     No     Multi Gather OpenSSH PKI Credentials Collection
   34  exploit/solaris/ssh/pam_username_bof                        2020-10-20       normal     Yes    Oracle Solaris SunSSH PAM parse_user_name() Buffer Overflow
   35  exploit/windows/ssh/putty_msg_debug                         2002-12-16       normal     No     PuTTY Buffer Overflow
   36  post/windows/gather/enum_putty_saved_sessions                                normal     No     PuTTY Saved Sessions Enumeration Module
   37  auxiliary/gather/qnap_lfi                                   2019-11-25       normal     Yes    QNAP QTS and Photo Station Local File Inclusion
   38  exploit/linux/ssh/quantum_dxi_known_privkey                 2014-03-17       excellent  No     Quantum DXi V1000 SSH Private Key Exposure
   39  exploit/linux/ssh/quantum_vmpro_backdoor                    2014-03-17       excellent  No     Quantum vmPRO Backdoor Command
   40  auxiliary/fuzzers/ssh/ssh_version_15                                         normal     No     SSH 1.5 Version Fuzzer
   41  auxiliary/fuzzers/ssh/ssh_version_2                                          normal     No     SSH 2.0 Version Fuzzer
   42  auxiliary/fuzzers/ssh/ssh_kexinit_corrupt                                    normal     No     SSH Key Exchange Init Corruption
   43  post/linux/manage/sshkey_persistence                                         excellent  No     SSH Key Persistence
   44  post/windows/manage/sshkey_persistence                                       good       No     SSH Key Persistence
   45  auxiliary/scanner/ssh/ssh_login                                              normal     No     SSH Login Check Scanner
   46  auxiliary/scanner/ssh/ssh_identify_pubkeys                                   normal     No     SSH Public Key Acceptance Scanner
   47  auxiliary/scanner/ssh/ssh_login_pubkey                                       normal     No     SSH Public Key Login Scanner
   48  exploit/multi/ssh/sshexec                                   1999-01-01       manual     No     SSH User Code Execution
   49  auxiliary/scanner/ssh/ssh_enumusers                                          normal     No     SSH Username Enumeration
   50  auxiliary/fuzzers/ssh/ssh_version_corrupt                                    normal     No     SSH Version Corruption
   51  auxiliary/scanner/ssh/ssh_version                                            normal     No     SSH Version Scanner
   52  post/multi/gather/saltstack_salt                                             normal     No     SaltStack Salt Information Gatherer
   53  exploit/unix/http/schneider_electric_net55xx_encoder        2019-01-25       excellent  Yes    Schneider Electric Pelco Endura NET55XX Encoder
   54  exploit/windows/ssh/securecrt_ssh1                          2002-07-23       average    No     SecureCRT SSH1 Buffer Overflow
   55  exploit/linux/ssh/solarwinds_lem_exec                       2017-03-17       excellent  No     SolarWinds LEM Default SSH Password Remote Code Execution
   56  exploit/linux/ssh/symantec_smg_ssh                          2012-08-27       excellent  No     Symantec Messaging Gateway 9.5 Default SSH Password Vulnerability
   57  exploit/linux/http/symantec_messaging_gateway_exec          2017-04-26       excellent  No     Symantec Messaging Gateway Remote Code Execution
   58  exploit/windows/ssh/sysax_ssh_username                      2012-02-27       normal     Yes    Sysax 5.53 SSH Username Buffer Overflow
   59  auxiliary/dos/windows/ssh/sysax_sshd_kexchange              2013-03-17       normal     No     Sysax Multi-Server 6.10 SSHD Key Exchange Denial of Service
   60  exploit/unix/ssh/tectia_passwd_changereq                    2012-12-01       excellent  Yes    Tectia SSH USERAUTH Change Request Password Reset Vulnerability
   61  auxiliary/scanner/ssh/ssh_enum_git_keys                                      normal     No     Test SSH Github Access
   62  exploit/linux/http/ubiquiti_airos_file_upload               2016-02-13       excellent  No     Ubiquiti airOS Arbitrary File Upload
   63  payload/cmd/unix/reverse_ssh                                                 normal     No     Unix Command Shell, Reverse TCP SSH
   64  exploit/linux/ssh/vmware_vdp_known_privkey                  2016-12-20       excellent  No     VMware VDP Known SSH Key
   65  exploit/multi/http/vmware_vcenter_uploadova_rce             2021-02-23       manual     Yes    VMware vCenter Server Unauthenticated OVA File Upload RCE
   66  exploit/linux/ssh/vyos_restricted_shell_privesc             2018-11-05       great      Yes    VyOS restricted-shell Escape and Privilege Escalation
   67  post/windows/gather/credentials/mremote                                      normal     No     Windows Gather mRemote Saved Password Extraction
   68  exploit/windows/local/unquoted_service_path                 2001-10-25       excellent  Yes    Windows Unquoted Service Path Privilege Escalation
   69  auxiliary/scanner/ssh/libssh_auth_bypass                    2018-10-16       normal     No     libssh Authentication Bypass Scanner
   70  exploit/linux/http/php_imap_open_rce                        2018-10-23       good       Yes    php imap_open Remote Code Execution


Interact with a module by name or index. For example info 70, use 70 or use exploit/linux/http/php_imap_open_rce
```
- 偵測 SSH 伺服器版本的模組，並查看該模組的相關參數 ==> 


## 攻擊jenkins
```
msf6 > search jenkins                                                                                                                                                                                   
                                                                                                                                                                                                
Matching Modules                                                                                                                                                                                        
================
   #   Name                                                  Disclosure Date  Rank       Check  Description
   -   ----                                                  ---------------  ----       -----  -----------
   0   exploit/windows/misc/ibm_websphere_java_deserialize   2015-11-06       excellent  No     IBM WebSphere RCE Java Deserialization Vulnerability
   1   exploit/multi/http/jenkins_metaprogramming            2019-01-08       excellent  Yes    Jenkins ACL Bypass and Metaprogramming RCE
   2   exploit/linux/http/jenkins_cli_deserialization        2017-04-26       excellent  Yes    Jenkins CLI Deserialization
   3   exploit/linux/misc/jenkins_ldap_deserialize           2016-11-16       excellent  Yes    Jenkins CLI HTTP Java Deserialization Vulnerability
   4   exploit/linux/misc/jenkins_java_deserialize           2015-11-18       excellent  Yes    Jenkins CLI RMI Java Deserialization Vulnerability
   5   post/multi/gather/jenkins_gather                                       normal     No     Jenkins Credential Collector
   6   auxiliary/gather/jenkins_cred_recovery                                 normal     Yes    Jenkins Domain Credential Recovery
   7   auxiliary/scanner/jenkins/jenkins_udp_broadcast_enum                   normal     No     Jenkins Server Broadcast Enumeration
   8   exploit/multi/http/jenkins_xstream_deserialize        2016-02-24       excellent  Yes    Jenkins XStream Groovy classpath Deserialization Vulnerability
   9   auxiliary/scanner/http/jenkins_enum                                    normal     No     Jenkins-CI Enumeration
   10  auxiliary/scanner/http/jenkins_login                                   normal     No     Jenkins-CI Login Utility
   11  exploit/multi/http/jenkins_script_console             2013-01-18       good       Yes    Jenkins-CI Script-Console Java Execution
   12  auxiliary/scanner/http/jenkins_command                                 normal     No     Jenkins-CI Unauthenticated Script-Console Scanner
   13  exploit/linux/misc/opennms_java_serialize             2015-11-06       normal     No     OpenNMS Java Object Unserialization Remote Code Execution                                     
Interact with a module by name or index. For example info 13, use 13 or use exploit/linux/misc/opennms_java_serialize

```
