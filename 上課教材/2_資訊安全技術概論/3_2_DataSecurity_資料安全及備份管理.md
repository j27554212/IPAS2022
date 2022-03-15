# 3_2_資料安全及備份管理

### 參考課程
```
Data Management, Recovery, Backup, Shredding & Encryption
Recover (Undelete) deleted data, explore backup options, data sanitization and shredding, encrypt your files
4.2 (40 個評等)  1217 名學生註冊  建立者： Hazem Salam 上次更新 4/2016
https://www.udemy.com/file-management-and-backup/

Introduction 11 堂講座 32:27
Data Recovery 7 堂講座 32:25
Data Backup  5 堂講座  21:42
Permanent Data Deletion (Data Sanitization): 8 堂講座  24:53
Data Encryption  5 堂講座  11:45
```
```
Master Data Management
An introductory course about understanding master data management, its building blocks and maturity model.
3.1 (147 個評等)  734 名學生註冊  建立者： The Art Of Service  上次更新 2/2018
https://www.udemy.com/master-data-management/
```
```
Data Warehousing 資料倉庫
An introductory course about understanding data warehousing, its architecture, flow, applications and modeling.
4.0 (47 個評等)  679 名學生註冊  建立者： The Art Of Service  上次更新 3/2015
https://www.udemy.com/data-warehousing/
```
```
Data Security
An introductory course about understanding Data Security and the different technologies involved in securing your data.
3.8 (17 個評等)  203 名學生註冊  建立者： The Art Of Service  上次更新 3/2015
https://www.udemy.com/data-security/
```
```
AWS Data Security
Carry out the best practices to protect your valuable data when working with data services on the Amazon cloud
0.0 (0 個評等)  21 名學生註冊  建立者： Packt Publishing 上次更新 7/2018
https://www.udemy.com/aws-data-security/
```
# DataSecurity_資料安全
```
What is Data Security?What does Data Security mean?
Why Data Security?
Data Security Solutions

https://software.microfocus.com/en-us/what-is/data-security
```
### Data Security(https://en.wikipedia.org/wiki/Data_security)
```
Data security means protecting digital data, such as those in a database, 
from destructive forces and from the unwanted actions of unauthorized users,such as a cyberattack or a data breach
```
```
Data security refers to protective digital privacy measures 
that are applied to prevent unauthorized access to computers, 
databases and websites. Data security also protects data from corruption. 
Data security is an essential aspect of IT for organizations of every size and type.

Data security is also known as information security (IS) or computer security.

What does Data Security mean?
https://software.microfocus.com/en-us/what-is/data-security
```

### Data Security:Technologies資料安全技術

```
[1]Disk encryption資料加密
Disk encryption refers to encryption technology that encrypts data on a hard disk drive. 
Disk encryption typically takes form in either software (see disk encryption software) or hardware (see disk encryption hardware). 
Disk encryption is often referred to as on-the-fly encryption (OTFE) or transparent encryption.

[2]Software versus hardware-based mechanisms for protecting data
Software-based security solutions encrypt the data to protect it from theft. 
However, a malicious program or a hacker could corrupt the data in order to make it unrecoverable, making the system unusable. 
Hardware-based security solutions can prevent read and write access to data and hence offer very strong protection against tampering and unauthorized access.

Hardware based security or assisted computer security offers an alternative to software-only computer security. 
Security tokens such as those using PKCS#11 may be more secure due to the physical access required in order to be compromised. 
Access is enabled only when the token is connected and correct PIN is entered (see two-factor authentication). 
However, dongles can be used by anyone who can gain physical access to it. 
Newer technologies in hardware-based security solves this problem offering full proof security for data.

Working of hardware-based security: A hardware device allows a user to log in, log out and 
set different privilege levels by doing manual actions. 
The device uses biometric technology to prevent malicious users from logging in, logging out, and changing privilege levels. 
The current state of a user of the device is read by controllers in peripheral devices such as hard disks. 

Illegal access by a malicious user or a malicious program is interrupted based on the current state of a user 
by hard disk and DVD controllers making illegal access to data impossible. 
Hardware-based access control is more secure than protection provided by the operating systems 
as operating systems are vulnerable to malicious attacks by viruses and hackers. 
The data on hard disks can be corrupted after a malicious access is obtained. 
With hardware-based protection, software cannot manipulate the user privilege levels. 
It is impossible for a hacker or a malicious program to gain access to secure data protected by hardware or perform unauthorized privileged operations. This assumption is broken only if the hardware itself is malicious or contains a backdoor.

The hardware protects the operating system image and file system privileges from being tampered. 
Therefore, a completely secure system can be created using a combination of hardware-based security 
and secure system administration policies.

[3]Backups資料備份
Backups are used to ensure data which is lost can be recovered from another source. 
It is considered essential to keep a backup of any data in most industries 
and the process is recommended for any files of importance to a user.

[4]Data masking資料渾淆
Data masking of structured data is the process of obscuring (masking) specific data within a database table or cell 
to ensure that data security is maintained and sensitive information is not exposed to unauthorized personnel. 

This may include masking the data from users (for example so banking customer representatives can only see the last 4 digits of a customers national identity number), developers (who need real production data to test new software releases but should not be able to see sensitive financial data), outsourcing vendors, etc. 

[5]Data erasure資料清除
Data erasure is a method of software based overwriting that completely destroys all electronic data residing on a hard drive or other digital media to ensure that no sensitive data is lost when an asset is retired or reused
```
### Data masking 資料渾淆
```
Data masking[1] or data obfuscation[2] is the process of hiding original data with random characters or data.

[Data Masking](https://www.techopedia.com/definition/13602/data-masking)
Data masking refers to the process of changing certain data elements within a data store 
so that the structure remains similar 
while the information itself is changed to protect sensitive information. 

Data masking ensures that sensitive customer information is unavailable beyond the permitted production environment. 
This is especially common when it comes to situations like user training and software testing.

https://en.wikipedia.org/wiki/Data_masking

```

### 資料安全:What You Can Do
```
[資料來源]https://dzone.com/articles/why-is-data-security-important-for-everyone

Remember, your awareness is your security. 
Here, I share the essential practices you need to start doing today to protect yourself from hackers:

Never click on spam, phishing, or a suspicious email. Verify or check an email or a link carefully before opening any attachment.

If something seems too good to be true, it probably is. 
Don’t fall prey to offers, such as "iPhone X at just $10" or "Congratulations! You won a car. Open attachment to claim now."

Never download any untrusted or pirated software or application.

Don’t download fake security software.

Use antivirus and/or firewalls

Don’t make any online transactions if the website is not secured. 
Check HTTPS or green address bar before making any payment or typing in any sensitive details

Use two-factor authentications.

Don’t share your personal or sensitive information to strangers.
```

# 資料不安全事件

# 備份管理BACKUP MANAGEMENT

## 備份 https://en.wikipedia.org/wiki/Backup
```
https://zh.wikipedia.org/wiki/%E5%A4%87%E4%BB%BD

在資訊科技與資料管理領域，備份指將檔案系統或資料庫系統中的資料加以複製；

一旦發生災難或錯誤操作時，得以方便而及時地恢復系統的有效資料和正常運作。

最好將重要資料製作三個，或三個以上的備份，並且放置在不同的場所異地備援，以利日後回存之用。
```
## 備份類型
```
全部備份（Full Backup）==>把硬碟或資料庫內的所有檔案、資料夾或資料作一次性的複製。
增量備份（Incremental Backup）==>對上一次全部備份或增量備份後更新的資料進行備份。
差異備份 (Differential backup) ==>差異備份提供執行完整備份後變更的檔案的備份
選擇式備份==>對系統的一部分進行備份。
冷備份==>系統處於停機或維護狀態下的備份。這種情況下，備份的資料與系統中此時段的資料完全一致。
熱備份==>系統處於正常運轉狀態下的備份。這種情況下，由於系統中的資料可能隨時在更新，備份的資料相對於系統的真實資料可有一定滯後。
```
## 備份類型
```
線上備份 (On-line Backup) : 需要及時還原的資料可以採用這總類型的備份，可以使用磁碟陣列、存儲區域網路、網路附加儲存或者是網路硬碟來保護資料安全。
離線備份 (Off-line Backup ): 離線備份使用可離線媒體來備份，磁帶、光碟或是硬碟盒備份完成後離開備份媒體。
```

## 各種資料處理的技術
```
在實施備份的過程中，可以對資料進行各種處理，這些不同的處理方式可以改善備份速度，恢復速度，增加資料安全性，提升儲存媒介的利用率。

資料壓縮技術（Compression）：通過各種機制來降低備份資料的大小，以便占用更少的儲存空間，壓縮的方法在磁帶儲存中尤為常見。

資料重複刪除技術（De-duplication）：當多個相似系統的資料要備份到同一台儲存裝置上時，需要重複備份資料，這會產生大量的冗餘。
例如，有20個Windows工作站要備份到同一台儲存裝置上，備份資料就可以共用系統檔案。
儲存裝置上只需要一份系統檔案，就可以用來恢復多個工作站。這項技術可以應用在檔案級，也可以應用在未經處理的資料塊級，
通過避免冗餘資料的重複複製，可以大大節省儲存裝置的儲存空間。重複資料刪除技術可以發生在伺服器端，在資料備份到儲存之前執行，
這種方法可以在節省儲存空間的同時節省備份資料的頻寬需求，這種方式的重複資料刪除叫做線上即時資料處理（inline）；
重複資料刪除技術也可以發生在儲存裝置端，稱之為後台重複資料刪除技術。

資料複製技術（Duplication）：在備份的過程中，資料有可能需要額外備份到第二組儲存裝置；
通過將備份資料複製，可以調整備份鏡像來最佳化恢復速度，而且可以將第二份備份資料存放在不同的備份地點，或不同的備份媒介上。

資料加密技術（Encryption）：對於大容量的抽取式的備份儲存媒介，例如磁帶，會面臨遺失和被盜的風險。
通過對資料加密可以降低上述風險，
但是也帶來了另外的問題：首先，加密會占用大量的CPU行程，從而降低了備份速度；
其次，資料被加密之後，就不能有效地壓縮，例如某些磁帶驅動器的資料壓縮技術無法實施。
基於上述原因，以及冗餘資料導致解密分析供給更加容易，很多加密技術都在實施之前進行壓縮；最後，加密技術要成功起作用，必須配合整體的安全策略通盤考慮。

資料緩衝技術（Staging）：利用資料緩衝技術，備份資料在複製到磁帶之前，會先複製到緩衝磁碟，這個操作稱之為D2D2T，磁碟到磁碟到磁帶。
資料緩衝技術（虛擬帶庫技術）在基於網路的備份系統中尤為重要，因為D2D2T技術可以緩解系統對於備份頻寬的需求。
如果備份系統中需要執行其他的資料操作，緩衝磁碟還可以起到資料中心的作用。
```
