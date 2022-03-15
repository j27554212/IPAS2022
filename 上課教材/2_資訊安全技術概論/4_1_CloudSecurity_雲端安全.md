# 4_1_雲端安全

```
雲端運算cloud computing
雲端資安事件
雲端資安威脅模型
雲端安全產品
```

#
```
Docker技術入門與實戰
基于最新Docker社区版，通过实际操作学习Docker,Docker Compose, Docker Swarm
4.2 (156 個評等)  1060 名學生註冊  建立者： Peng Xiao  上次更新 8/2018
https://www.udemy.com/docker-china/
```

```
Docker and Kubernetes: The Complete Guide
Build, test, and deploy Docker applications with Kubernetes while learning production-style development workflows
4.7 (1694 個評等)  11469 名學生註冊  建立者： Stephen Grider  上次更新 10/2018
https://www.udemy.com/docker-and-kubernetes-the-complete-guide/
```
```
Kubernetes技术入门与实战
通过实际操作讲解Kubernetes基本概念和使用
4.6 (31 個評等)  193 名學生註冊  建立者： Peng Xiao  上次更新 10/2018
```
```
Learn DevOps: Advanced Kubernetes Usage
Covering Authentication, Authorization, Logging, Helm, Deploying with Spinnaker, Prometheus, Scheduling and more
4.2 (425 個評等)  7718 名學生註冊  建立者： Edward Viaene  上次更新 8/2018
https://www.udemy.com/learn-devops-advanced-kubernetes-usage/
```

# 雲端運算cloud computing

### 定義
```
NIST SP800-145== NIST Special Publication (SP) 800-145
The NIST Definition of Cloud Computing
https://nvlpubs.nist.gov/nistpubs/legacy/sp/nistspecialpublication800-145.pdf
```
### NIST==National Institute of Standards and Technology==美國國家標準暨技術研究院
```
美國國家標準暨技術研究院（National Institute of Standards and Technology，簡寫為NIST）
前身為國家標準局（NBS，1901年~1988年），
是一家測量標準實驗室，屬於美國商務部的非監管機構。該研究所的官方使命為：
Promote U.S. innovation and industrial competitiveness by advancing measurement science, standards, 
and technology in ways that enhance economic security and improve our quality of life.
促進美國的創新和產業競爭力，推進度量衡學、標準、技術以提高經濟安全並改善我們的生活質量。

NIST僱傭有大約2900名科學家、工程師、科技工作者，以及後勤和管理人員，
大約1800名輔助工作人員（來自美國公司和國外的工程師和研究員），
另外還有1400名專家分布在國內約350個附屬研究中心裡。
```

### 雲端運算五大特色 five Essential Characteristics of Cloud Computing 

[1]On-demand self-service. 
```
A consumer can unilaterally provision computing capabilities, such as server time and network storage, 
as needed automatically without requiring human interaction with each service provider.
```
[2]Broad network access. 
```
Capabilities are available over the network and accessed through standard mechanisms that promote use by 
heterogeneous thin or thick client platforms (e.g., mobile phones, tablets, laptops, and workstations).
```
[3]Resource pooling. 
```
The provider’s computing resources are pooled to serve multiple consumers using a multi-tenant model, 
with different physical and virtual resources dynamically assigned and reassigned according to consumer demand. 
There is a sense of location independence in that the customer generally has no control or knowledge over the exact
location of the provided resources but may be able to specify location at a higher level of
abstraction (e.g., country, state, or datacenter). Examples of resources include storage,
processing, memory, and network bandwidth.
```
[4]Rapid elasticity. 
```
Capabilities can be elastically provisioned and released, in some cases automatically, 
to scale rapidly outward and inward commensurate with demand. 
To the consumer, the capabilities available for provisioning often appear to be unlimited and can
be appropriated in any quantity at any time.
```
[5]Measured service. 
```
Cloud systems automatically control and optimize resource use by leveraging a metering capability
at some level of abstraction appropriate to the type of service (e.g., storage, processing, bandwidth, 
and active user accounts). Resource usage can be monitored, controlled, and reported, providing 
transparency for both the provider and consumer of the utilized service.
```

### 雲端運算類型==服務模型Service Models:

[1]Software as a Service (SaaS)==> Gmail, office 365,  youtube, facebook,
```
The capability provided to the consumer is to use the provider’s applications running on a cloud infrastructure. 
The applications are accessible from various client devices through either a thin client interface, 
such as a web browser (e.g., web-based email), or a program interface. The consumer does not manage or control the
underlying cloud infrastructure including network, servers, operating systems, storage, or
even individual application capabilities, with the possible exception of limited userspecific
application configuration settings.
```
[2]Platform as a Service (PaaS)==> Google Cloud platform, Microsoft Azure Platform, Amazon Web Services Cloud
```
The capability provided to the consumer is to deploy onto the cloud infrastructure consumer-created or acquired applications 
created using programming.
Typically this is done on a pay-per-use or charge-per-use basis. 
A cloud infrastructure is the collection of hardware and software that enables the five essential characteristics of cloud
computing. 
The cloud infrastructure can be viewed as containing both a physical layer and an abstraction layer. 
The physical layer consists of the hardware resources that are necessary to support the cloud services being provided, 
and typically includes server, storage and network components. 
The abstraction layer consists of the software deployed across the physical layer,
which manifests the essential cloud characteristics. Conceptually the abstraction layer sits above the physical layer.
languages, libraries, services, and tools supported by the provider.

The consumer does not manage or control the underlying cloud infrastructure including network, servers,
operating systems, or storage, but has control over the deployed applications and possibly
configuration settings for the application-hosting environment.
```
[3]Infrastructure as a Service (IaaS)==> Google Cloud platform, Microsoft Azure Platform, Amazon Web Services Cloud
```
The capability provided to the consumer is to provision processing, storage, networks, and other fundamental computing resources 
where the consumer is able to deploy and run arbitrary software, which can include operating systems and applications. 
The consumer does not manage or control the underlying cloud infrastructure but has control over operating systems, 
storage, and deployed applications; and possibly limited control of select networking components (e.g., host firewalls).
```

### 雲端運算部屬模型Deployment Models:

[1]Private cloud私有雲
```
The cloud infrastructure is provisioned for exclusive use by a single organization comprising multiple consumers (e.g., business units). 
It may be owned, managed, and operated by the organization, a third party, or some combination of them, and it may exist
on or off premises.
```

[2]Community cloud.社群雲 
```
The cloud infrastructure is provisioned for exclusive use by a specific community of consumers from organizations 
that have shared concerns (e.g., mission, security requirements, policy, and compliance considerations). 
It may be owned, managed, and operated by one or more of the organizations in the community, a third
party, or some combination of them, and it may exist on or off premises.
```

[3]Public cloud.公有雲
```
The cloud infrastructure is provisioned for open use by the general public. 
It may be owned, managed, and operated by a business, academic, or government organization, or
some combination of them. It exists on the premises of the cloud provider.
```
[4]Hybrid cloud.混合雲 
```
The cloud infrastructure is a composition of two or more distinct cloud
infrastructures (private, community, or public) that remain unique entities, but are bound
together by standardized or proprietary technology that enables data and application
portability (e.g., cloud bursting for load balancing between clouds).
```

# NIST Cloud Computing Reference Architecture (CCRA)
```
NIST SP 500-292 
NIST Cloud Computing Reference Architecture
https://bigdatawg.nist.gov/_uploadfiles/M0008_v1_7256814129.pdf

NIST SP 500-291,Version 2(2013)
NIST Cloud Computing Standards Roadmap 
https://www.nist.gov/sites/default/files/documents/itl/cloud/NIST_SP-500-291_Version-2_2013_June18_FINAL.pdf

NIST SP 500-322 
Evaluation of Cloud Computing Services Based on NIST 800-145
https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.500-322.pdf
```
### 五大參與腳色:The five major participating actors 
```
[1]the Cloud Consumer
[2]Cloud Provider
[3]Cloud Broker
[3]Cloud Auditor 
[5]Cloud Carrier
```
# 雲端資安事件

```
```

# 雲端服務安全
底下從六大面向考量
```
[1]資安管理及安全性驗證
[2]資料儲存安全
[3]雲端作業系統與虛擬化安全
[4]傳輸安全防護
[5]應用安全
[6]實體安全
```
### (一)資安管理及安全性驗證所需技術

```
包含：安全成熟度等級與稽核、資安管理與稽核、系統監控機制、法規遵循、安全認證：
1.安全成熟度等級與稽核：
   雲端安全聯盟(CSA) 制定STAR認證來檢核服務供應商的安全性績效，以評估與其稽核服務供應商雲端安全管理的成熟度。
2.資安管理與稽核：如ISO27001資安管理與稽核於實體與環境安全、通訊與作業管理、存取控制、資訊系統獲取、開發及維護等資訊資產安全進行安全管理管制機制。
3.系統監控機制：為確保雲端服務的安全，制定系統的監控機制，以確保系統的安全。
4.法規遵循：由於各組織所處行業屬性或是國情不同，法規要求也有所不同；
   雲端安全聯盟(CSA)的雲端運算關鍵領域安全指南中，建議以企業風險管理、企業治理、及法規遵循與稽核要求此三個面向加以探討。
5.安全認證：常見的技術包含智能卡的使用者身份驗證、一次性密碼驗證、Kerberos認證、生物特徵驗證。
```
###  (二)資料儲存安全所需技術
```
包含：金鑰管理、完整性的驗證、資料加解密技術、資料備份/遺失防護、資料刪除安全性/資料隱私：
1.金鑰管理：金鑰管理包含技術與管理兩個層面，其囊括了金鑰的生成、配發、驗證、儲存、備份、維護、更新以及銷毀。
2.完整性的驗證 ：為防止資料在傳輸過程中遭受中間人攻擊，驗證檔案與原始檔案是否相同，其常見係使用加密雜湊演算法如MD5、SHA-1。
3.資料加解密技術 ： 加密技術主要分為對稱與非對稱兩種，其中著名的對稱式加密技術包含DES、Triple DES、AES、Blowfish、IDEA、RC5、RC6，
      而非對稱式加密技術包含RSA、ElGamal、背包演算法、Rabin、ECC以及迪菲－赫爾曼金鑰交換協定中的公鑰加密演算法。
4.資料備份/遺失防護 ： 為確保資料的安全，因將資料進行異地備援，避免資料的遺失與損會，目前許多雲端服務接預設含有此項目。
5.資料刪除安全性/資料隱私：在雲端架構底下，使用者刪除資料時，無法確保雲端服務商是否將實體資料刪除，
    因此企業需深入調查與了解，資料刪除的安全性與資料隱私性的議題。
```
### (三)雲端作業系統與虛擬化安全所需技術
```
包含：雲端作業系統(OpenStack)安全性、Docker技術安全性、Image安全檢測、特殊配置的安全、
      狀態恢復的安全、Hypervisor安全機制、虛擬機隔離機制安全分析：
1.雲端作業系統(OpenStack)安全性 ：OpenStack官方本生會維護兩個穩定版本，並即時更新安全漏洞。
    然而其安全性仍需持續觀察，建議架設監控系統並針對其原始碼進行嚴密的審查以確保其安全性。
2.Docker技術安全性 ： Docker的安全性主要仰賴隔離機制的安全性。並且Docker的Image建置容易，
    公開的倉庫(Repository)存在多個不安全的容器(Container)。為解決以上問題即需制定安全策略，並針對其原始碼進行嚴密的審查以確保其安全性
3.Image安全檢測：虛擬化技術通常將虛擬機以文件的格式儲存於主機之中，倘若Image本身未進行加密保護，
   將造成資料的外洩或被駭客修改，因此應針對Image安全進行嚴密的檢測。
4.特殊配置的安全： 虛擬機於應用上通常會安裝較舊的版本系統，因此虛擬機的系統配置將成為虛擬化的安全隱憂，
   因此企業應制定安全策略，確保虛擬機器的配置安全。
5.狀態恢復的安全：虛擬機中的資料通常以文件格式儲存於伺服器上，當虛擬機發生變動時，
  會採用快照技術以紀錄虛擬機的狀態與內容。因此虛擬機的狀態資料將會儲存於伺服器中，這為虛擬化安全帶來新的挑戰課題，
  如使用者會將系統還原不安全的系統版本或缺乏抵抗力的狀態。
6.Hypervisor安全機制 ： 
   Hypervisor主要分為建構輕量級的Hypervisor以及對Hypervisor進行完整性保護兩個安全的研究方向。
7.虛擬機隔離機制安全分析 ： 
  虛擬機隔離機制是虛擬化平臺安全性指標之一，透過隔離機制確保虛擬機之間獨立運行。
  目前虛擬機隔離機制研究多以Xen為基礎，而Xen有諸多安全漏洞，特別是Xen依賴VM0管理虛擬機所引發之漏洞，使惡意使用者可在虛擬機內部或外部進行攻擊。
```
### (四)傳輸安全防護所需技術
```
包含：資料傳輸安全技術、DDoS安全防護、APT安全防範：
1.資料傳輸安全技術 : 為確保傳輸安全通常採用SSL、VPN加密傳輸，可同時對資料本身增加加密機制。
2.DDoS安全防護 :DDoS攻擊非單一資安設備可完整防禦，需透過縱深防禦機制聯合防制。
  各家公司都推出相對應的關鍵技術，以下為
  全球知名產品評鑑網站TopTenReviews評比2016年十大DDoS防護產品：
  Incapsula  Enterprise、F5 Networks Silverline、Arbor Cloud、Nexusguard、Verisign DDoS Protection Service、
  Neustar SiteProtect、Akamai Kona Site Defender、DOSarrest Proxy Defense、CloudFlare Enterprise、
  Radware Attack Mitigation System。
3.APT安全防範 : 進階持續性威脅（APT）通常長時間潛伏在網路或系統內來達成目的，
   應加強端點防護，以偵測可疑電子郵件或內部主機異常行為，以預防APT滲透攻擊。
```
### (五)應用安全
```
所需技術包含：網頁與網站的安全性、應用程式搬移安全、資料內容安全性機制：
1.網頁與網站的安全性 : 網頁與網站的安全可參照OWASP Web Top10進行安全性的檢測，以便免常見的網頁式攻擊如XXS、Injection等。
2.應用程式搬移安全 : 企業應評估遷移所需之成本，包含本身成本以及營運成本，企業應訂定安全的搬移規範。
3.資料內容安全性機制 : 需檢驗雲端服務中的應用程式對於資料內容的儲存與處理是否有使用安全的加密技術，以及開發規範，避免資料的洩漏、竄改或損毀。
```
### (六)實體安全
```
所需技術包含：電磁洩漏防範機制、設備保護機制、設備防盜機制、環境的安全防範：
1.電磁洩漏防範機制 : 內裝修材料應避免毛毯、地毯等吸塵並且容易產生靜電之材料，並制定一定的安全流程。
2.設備保護機制 : 設備會遭遇人為、天災等資料的損壞，因此應制定設備的保護機制，確保設備的安全。
3.設備防盜機制 : 資料中心因設立嚴謹的管理條例並嚴格執行，避免設備被不明人士盜取。
4.環境的安全防範 : 資料中心的環境需避免火災發生、潮濕、落雷、電磁場干擾、高樓或地下室並遠離輻射源，避免實體設備遭環境損毀。
```
# 巨量資料安全   
```
巨量資料安全上，相關安全需考量：資安管理及安全性驗證、資料儲存安全、分散式運算框架的安全性、資料的隱私權與保護、端點資料的安全性:
```
### (一)資安管理及安全性驗證
```
所需技術包含：資安管理與稽核、安全成熟度等級與稽核、實體安全及系統監控機制、Data Center的安全性：
1.資安管理與稽核 : 為確保雲端福的安全性應定期進行資安的檢測如滲透測試。
2.安全成熟度等級與稽核 : 資訊安全管理應制定安全成熟度等級並定期針對服務進行安全稽核，以確保服務的安全性。
3.實體安全及系統監控機制 : 資料中心應制定實體安全的保護機制以及系統監控機制，以確保實體與系統接受到保護。
4.Data Center的安全性 : 資料中心的安全性是個非常龐大且複雜的安全性課題，需針對該中心進行安全項目的檢核
  包含網路安全、伺服器安全性、資料保護、應用程式安全、安全管理、安全性情報等。
```
### (二)資料儲存安全
```
所需技術包含：分散式檔案系統安全、關聯性資料庫安全、NoSQL資料庫安全、異動記錄檔安全：
1.分散式檔案系統安全 : 分散式檔案系統如著名的HDFS有自身的安全性機制，然而其安全性仍需持續觀察，
   建議架設監控系統並針對其原始碼進行嚴密的審查以確保其安全性。
2.關聯性資料庫安全 : 關聯式資料庫安全的原則除須滿足機密性、完整性、可用性、身份驗證、
  存取授權以及操作不可否認(Non-repudiation) 等安全需求。
  可參考Oracle 與SQL Server安全機制提出企業須將以下安全事項列入考量:
  稽核機制、授權與檢查機制、檢視機制、觸發機制、加密機制、資料備份與復原機制和備份、復原和控制機制。
3.NoSQL資料庫安全 : 
   NoSQL 資料庫缺少Schema因此難以進行完善的完整性檢驗，同時NoSQL為提高處理效率並未每次交易皆進行同步處理，影響其資料的正確性
   目前多數的NoSQL資料庫並沒有提供安全機制，因此建利用外部應用程式將資料加密，並進行原始碼檢測，以確保NoSQL的安全性。
4.異動記錄檔安全 : 系統異動時會產生記錄檔，應針對異動記錄檔訂定安全的管理規範。
```
### (三)分散式運算框架的安全性
```
所需技術包含：Storm平臺安全、Spark平臺安全，Hadoop平臺安全，詳如下列說明：
1.Storm平臺安全 : Storm因安全性機制的考量預設資料得授權語認證皆被禁止，因此使用時須進行嚴密的全線控管。
    然而其安全性仍需持續觀察，建議架設監控系統並針對其原始碼進行嚴密的審查以確保其安全性。
2.Spark平臺安全 : Spark可與Hadoop/YARN安全模型相容，進而確保其通訊的安全性。
    然而其安全性仍需持續觀察，建議架設監控系統並針對其原始碼進行嚴密的審查以確保其安全性。
3.Hadoop平臺安全 : Hadoop有自身的安全性機制如MapReduce添加ACL管理、所有task以作業擁有者身份運行、
   DistribuedCache設定private模式將利用Kerberos進行身分認證。
   然而其安全性仍需持續觀察，建議架設監控系統並針對其原始碼進行嚴密的審查以確保其安全性。
```
### (四)資料的隱私權與保護
```
所需技術包含：隱私洩漏安全防範、資料探勘安全性、法規遵循、加密演算法、傳輸安全：
1.隱私洩漏安全防範 : 資料儲存時應針對隱私資料進行安全的防範機制，包含加密技術、存取權限控管等。
2.資料探勘安全性 : 資料探勘時應將資料進行適當的分類，以避免分析時參入敏感性資訊，引發資料洩漏之疑慮。
3.法規遵循 : 各國法規不同，需確保雲端符合該國家的安全法規，避免法律上的糾紛。
4.加密演算法 : 加密技術主要分為對稱與非對稱兩種，
  其中著名的對稱式加密技術包含DES、Triple DES、AES、Blowfish、IDEA、RC5、RC6，
  非對稱式加密技術包含RSA、ElGamal、背包演算法、Rabin、ECC以及迪菲－赫爾曼金鑰交換協定中的公鑰加密演算法。
5	傳輸安全 : 為確保傳輸安全通常採用SSL、VPN加密傳輸，可同時對資料本身增加加密機制。
```
### (五)端點資料的安全性
```
所需技術包含：端點資料過濾、端點輸入驗證、資料完整性驗證：
1.端點資料過濾 : 為避免惡意攻擊者的Injection攻擊，針對輸入資料進行資料過濾。
2.端點輸入驗證 : 針對存取的使用者進行身份認證，並限制其僅可存取對應之資訊。
3.資料完整性驗證 :為防止資料在傳輸過程中遭受中間人攻擊，驗證檔案與原始檔案是否相同，其常見係使用加密雜湊演算法如MD5、SHA-1。
```

# CCSP雲端資安專家認證

CCSP==Certified Cloud Security Professional

```
https://www.uuu.com.tw/Course/Show/1146/CCSP雲端資安專家認證
https://spring-consultant.com/ccsp雲端安全專家認證輔導課程

雲端技術乃新世代資訊科技的基礎。作為新世代的資訊科技人，若不能掌握雲端技術則勢必被接下來的時代淘汰。
雲端技術擁有其有別於傳統資訊科技的特性，如軟體思維、快速彈性、低整體擁有成本及資源共享等特性。

然而，雲端技術的便利性，同時加深人們對於雲端技術的依賴，當新一代資訊科技變得如同傳統水電一般的呼之即來、揮之即去時，
這也意味著當系統中斷、服務停止時，人們將承受莫大損害，而這也暗示著雲端安全的重要性。

CCSP®認證是二大安全組織 – (ISC)2及CSA (雲端安全聯盟)兩大國際原廠聯手打造的頂級雲端資安認證。
透過此認證，主要用於表彰其持有者於資訊及雲端安全的專業與能力。藉此以協助組織維持重要雲端基礎設施的正常運作、免於危害。其切入點由架構開始，

由雲端平台與基礎設施往上堆疊，包含雲端應用程式與資料安全性，
更從考量設計到作業層面與法令、法規要求，以協助組織建構、維運雲端技術平台。

Domain 1：Architectural Concepts & Design Requirements架構觀念與設計要求

Domain 2：Cloud Data Security雲端資料安全性
Domain 3：Cloud Platform & Infrastructure Security雲端平台與基礎設施安全性
Domain 4：Cloud Application Security雲端應用程式安全性

Domain 5：Operations雲端作業
Domain 6：Legal & Compliance法律與遵循性

了解雲端運算的基本觀念與知識
了解雲端基礎架構與平台之設計與安全議題
了解雲端應用程式設計之要求與安全議題
了解雲端日常維運之重點與議題
了解與雲端相關之法令法規議題
具備考取(ISC)2-CCSP 之基礎知識

課程大綱
雲端基礎概念
設計原則
資料分類
雲端資料安全
雲端安全議題
角色與責任劃分
雲端應用安全
維運安全
法令法規要求
```
