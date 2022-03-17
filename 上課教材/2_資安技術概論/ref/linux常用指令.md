#
```
第 1章　登錄、退出、關機和重啟　1
1.1　login：使用者登錄系統　1
1.2　logout：退出登錄Shell　1
1.3　nologin：限制用戶登錄　1
1.4　exit：退出Shell　2
1.5　sulogin：單用戶登錄　2
1.6　rlogin：遠端登入　2
1.7　poweroff：關閉系統　3
1.8　ctrlaltdel：設置按Ctrl+Alt+Del複合鍵的功能　3
1.9　shutdown：關閉或重啟Linux系統　4
1.10　halt：關閉系統　5
1.11　reboot：重啟Linux系統　5
1.12　init：切換系統運行級別　6
1.13　runlevel：輸出以前和當前的運行級別　6
1.14　telinit：更改系統運行級別　7


第 2章　獲取幫助　8
2.1　help：查看內部Shell命令説明資訊　8
2.2　man：顯示線上手冊頁　8
2.3　manpath：查看和設置man手冊頁的查詢路徑　11
2.4　info：閱讀info格式的檔　11
2.5　pinfo：基於lynx類型info流覽　13

第3章　文字編輯器　15
3.1　vi：文字編輯器　15
3.2　nano：nano編輯器　20
3.3　view：文字編輯器　22
3.4　ex：文字編輯器　22
3.5　ed：文字編輯器　22
3.6　red：文字編輯器　23
3.7　emacs：GNU專案編輯器　24

第4章　目錄和檔操作 　25

4.1　pwd：顯示當前工作目錄路徑　25
4.2　cd：更改工作目錄路徑　25
4.3　ls：列出目錄和檔資訊　26
4.4　dir：列出目錄或檔資訊　28
4.5　dirs：顯示目錄清單　31
4.6　touch：創建空檔或更改檔時間　32

4.7　mkdir：創建目錄　33
4.8　rmdir：刪除空目錄　33
4.9　cp：複製檔和目錄　34
4.10　mv：檔和目錄改名、移動檔和目錄路徑　34
4.11　rm：刪除檔或目錄　35

4.12　install：複製檔和設置屬性　35
4.13　tmpwatch：刪除在指定時間段內沒有被訪問的檔　36
4.14　file：查詢檔案類型　37
4.15　du：顯示目錄或檔的磁片占用量　38
4.16　wc：統計檔行數、單詞數、位元組數和字元數　39
4.17　tree：以樹狀圖逐級列出目錄的內容　40
4.18　cksum：顯示檔的CRC校驗值和位元組統計　42
4.19　md5sum：顯示或檢查MD5校驗和　42
4.20　sum：為檔輸出校驗和及塊計數　43
4.21　dirname：輸出去除尾部的“/”字元部分的名稱　43
4.22　mkfifo：創建FIFO文件　43
4.23　mktemp：創建暫存檔案或目錄　44
4.24　ln：創建連結檔　44
4.25　sln：靜態ln　45
4.26　lndir：創建一個連結到另一個目錄樹的符號連結的影子目錄　45
4.27　link：調用link函數來創建檔連結　46
4.28　unlink：調用unlink函數刪除指定的檔 　46
4.29　basename：去掉前導的目錄部分後顯示名稱　46
4.30　pathchk：檢查檔案名是否有效或可擕式　47
4.31　symlinks：檢查目錄中的符號連結　47
4.32　stat：顯示檔或檔案系統狀態　48
4.33　rcp：遠程檔複製 　50
4.34　fsview：檔案系統流覽器　50
4.35　mc：類UNIX作業系統的目錄流覽器/檔案管理員　52

第5章　顯示文字檔內容　53
5.1　cat：顯示文字檔　53
5.2　more：分頁顯示文字檔　54
5.3　less：回卷顯示文字檔　56
5.4　head：顯示指定檔前若干行　58
5.5　tail：查看檔末尾資料　60
5.6　nl：顯示檔的行號和檔內容　61
5.7　tac：從**後一行開始顯示檔內容　63
5.8　rev：把每一行字元的順序顛倒過來顯示檔內容　63
5.9　fold：限制檔列寬顯示檔內容　64
5.10　fmt：簡單優化文本格式 　64
5.11　expand：將檔中的定位字元轉換為空格寫到標準輸出　65
5.12　pr：對指定檔附注列印所需的頁碼或聚焦　65

第6章　文件處理　67
6.1　sort：對檔中的資料進行排序　67
6.2　uniq：將重複行從輸出檔中刪除　67
6.3　cut：從檔每行中輸出選定的位元組、字元或欄位　68
6.4　comm：逐行比較兩個已排序的文件　70
6.5　diff：逐行比較兩個文字檔，列出其不同之處　71
6.6　join：每一對具有相同內容的輸入行整合為一行　72
6.7　diff3：按行比較3個文件　73
6.8　cmp：按位元組比較兩個檔　74
6.9　colrm：從檔中刪除列　75
6.10　paste：合併檔的行　75
6.11　tr：從標準輸入中替換、縮減和/或刪除字元　76
6.12　split：檔分割成片　77
6.13　csplit：按照指定的格式將檔分塊為“xx00”、“xx01”...並輸出　78
6.14　tee：將標準輸入複製到每個指定檔　79
6.15　unexpand：空格字元轉換為定位字元 　79
6.16　patch：應用一個diff檔　80
6.17　awk：模式掃描和處理語言　81
6.18　sed：用於過濾和轉換文本的流編輯器　85
6.19　od：以八進制和其他格式轉儲檔　88

第7章　字串、檔和命令查找　91
7.1　grep：查找檔中符合條件的字串　91
7.2　egrep：在檔或標準輸入中查找模式　93
7.3　fgrep：在每個檔或是標準輸入中查找模式　94
7.4　find：列出檔案系統內符合條件的檔　95
7.5　updatedb：創建或更新mlocate資料庫　98
7.6　locate：在資料庫中查找檔　98
7.7　whereis：查找指定文件、命令和手冊頁位置　99
7.8　whatis：在whatis資料庫中搜尋特定命令　100
7.9　apropos：搜索whatis資料庫中的字串　100
7.10　which：顯示可執行命令的路徑　100
7.11　look：顯示指定字串的行開頭　101

第8章　日期和時間　102
8.1　cal：顯示日曆資訊　102
8.2　date：顯示和設置系統日期和時間　103
8.3　hwclock：查看和設置硬體時鐘　105
8.4　clock：查看和設置硬體時鐘　105
8.5　clockdiff：主機之間測量時鐘差　106
8.6　zdump：時區輸出器　106
8.7　rdate：通過網路獲取時間　107
8.8　sleep：暫停指定的時間　108

第9章　數字計算　109

9.1　bc：任意精度的計算器　109
9.2　dc：一個任意精度的計算器　109
9.3　expr：將運算式的值列印到標準輸出　110

第 10章　Shell相關命令　112
10.1　command：抑制正常的Shell函數查找　112
10.2　exec：使用執行命令替換當前的Shell進程　112
10.3　bash：GNU的Bourne-Again Shell　112
10.4　builtin：執行Shell內建命令　113
10.5　enable：啟用或禁用內建Shell命令　113
10.6　source：在當前Shell環境中從指定檔讀取和執行命令　115
10.7　mksh：用於互動式和Shell腳本的命令直譯器　115
10.8　suspend：暫停Shell執行　115
10.9　sushell：執行單用戶Shell　116
10.10　shopt：切換變數控制可選的Shell行為的值　116
10.11　rsh：遠程Shell　117
10.12　ulimit：控制Shell執行程式的資源使用限制　117
10.13　history：查看命令歷史記錄　119
10.14　alias：查看和定義別名　120
10.15　unalias：取消別名　120
10.16　eval：連接指定參數在一起成為一個單一的命令來執行　121
10.17　fc：修改或執行命令　121

第 11章　Shell程式設計　122
11.1　declare：顯示或設置Shell變數 　122
11.2　export：顯示或設置環境變數　123
11.3　set：顯示和設置Shell變數　123
11.4　unset：刪除變數或函數　124
11.5　env：查看和設置環境變數　125
11.6　read：從標準輸入中讀取一行　125
11.7　readonly：設置唯讀變數　126
11.8　test： 檢查檔案類型，並比較值 　126
11.9　false：什麼都不做，表示失敗　129

第 12章　程式編譯　130

12.1　gcc：GNU項目的C和C+ +編譯器　130
12.2　gdbserver：為GNU調試的遠端伺服器 　131
12.3　cmake：跨平臺Makefile生成工具 　131
12.4　indent：更改通過插入或刪除空格的C程式外觀 　132
12.5　protoize：自動添加函數原型　134
12.6　unprotoize：自動刪除函數原型　135
12.7　gcov：顯示代碼覆蓋資訊　135
12.8　find2perl：轉換找到的命令列為Perl代碼 　136
12.9　as：可擕式GNU組合語言程式　137
12.10　php：PHP命令列介面　139
12.11　perl：實用報表提取語言　140
12.12　gdb：GNU調試器　142
12.13　autoupdate：更新configure.in到較新的Autoconf 　144
12.14　autoheader：創建C定義的範本檔　145
12.15　autoreconf：更新已經生成的設定檔　145
12.16　autoscan：生成一個初步的configure.in 　146
12.17　autoconf：從範本檔生成配置腳本　146

第 13章　用戶和組群管理　148
13.1　useradd：創建用戶帳戶　148
13.2　adduser：創建用戶帳戶　149
13.3　lnewusers：創建用戶帳戶　149
13.4　usermod：修改用戶帳戶 　149
13.5　userdel：刪除用戶帳戶 　150
13.6　groupadd：創建組群　151
13.7　groupmod：修改組群　151
13.8　groupdel：刪除組群　152
13.9　passwd：設置或修改使用者密碼　152
13.10　gpasswd：設置組群密碼或在組群中添加、刪除用戶　153
13.11　chfn：更改finger信息　154
13.12　chsh：更改用戶帳戶的Shell類型　155
13.13　pwck：校驗/etc/passwd 和/etc/shadow檔的內容是否合法和完整　155
13.14　newgrp：讓用戶帳戶以另一個組群的身份進行登錄　156
13.15　finger：使用者資訊查找程式　157
13.16　groups：顯示指定使用者帳戶的組群成員身份　157
13.17　id：顯示使用者的UID及該用戶所屬組群的GID　158
13.18　grpck：驗證組群檔的完整性　158
13.19　grpconv: 啟用組群影子密碼　159
13.20　grpunconv：關閉組群的影子密碼　159
13.21　groupmems：管理用戶主要組群的成員　159
13.22　userinfo：更改自己的finger資訊　160
13.23　userpasswd：允許使用者更改密碼的圖形化工具　160
13.24　vigr：編輯/etc/group檔　161
13.25　vipw：編輯/etc/passwd、/etc/shadow、/etc/group和/etc/gshadow檔　162
13.26　newusers：更新和批量創建新用戶 　162
13.27　chpasswd：成批更新用戶口令　163
13.28　pwconv：開啟影子密碼功能　163
13.29　pwunconv：關閉影子密碼功能　164
13.30　chage：更改使用者密碼到期資訊　164
13.31　su：切換到其他用戶帳戶進行登錄　165
13.32　visudo：編輯/etc/sudoers檔　166
13.33　sudo：以另外一個用戶執行命令　166
13.34　sudoedit：以另外一個用戶身份編輯檔　167
13.35　sudoreplay：重播sudo會話日誌　168

第 14章　顯示登錄使用者　169
14.1　w：詳細查詢已登錄當前電腦的使用者　169
14.2　who：顯示已登錄當前電腦使用者的簡單資訊　169
14.3　whoami：顯示與當前的有效使用者ID相關聯的用戶名　170
14.4　logname：顯示當前使用者的登錄名稱　170
14.5　users：用單獨的一行顯示出當前登錄的使用者　171
14.6　last：顯示近期使用者登錄情況　171
14.7　lastb：列出登錄系統失敗的使用者資訊　173
14.8　lastlog：查看用戶上次登錄的時間　173
14.9　rwho：顯示在本地網路的所有主機上登錄的使用者資訊　174

第 15章　檔、目錄許可權和屬性　175
15.1　chmod：更改檔和目錄的模式　175
15.2　chown：更改檔和目錄的使用者所有者和組群所有者　177
15.3　chgrp：更改檔或目錄的所屬組　177
15.4　umask：顯示和設置檔及目錄創建預設許可權遮罩　178
15.5　getfacl：顯示檔或目錄的ACL　179
15.6　setfacl：設置檔或目錄的ACL　179
15.7　chacl：更改檔或目錄的ACL　181
15.8　lsattr：查看檔和目錄的屬性　181
15.9　chattr：更改檔和目錄的屬性　182

第 16章　歸檔與壓縮　183
16.1　tar：進行歸檔和壓縮　183
16.2　gzip：壓縮或解壓縮gzip檔　185
16.3　gunzip：解壓縮gzip檔　186
16.4　zcmp：比較gzip壓縮檔　187
16.5　zdiff：比較gzip壓縮檔　187
16.6　zforce：在所有的gzip檔上強制添加.gz擴展　188
16.7　zip：壓縮zip檔　188
16.8　unzip：解壓縮 zip檔　190
16.9　zcat：查看zip壓縮檔　190
16.10　zgrep：在壓縮檔中按規則運算式來搜索　191
16.11　zipgrep：在zip壓縮檔中搜索匹配指定的字串或模式　191
16.12　zipinfo：列出zip檔相關的詳細資訊　192
16.13　zipsplit：拆分zip文件　192
16.14　zless：查看zip壓縮檔　193
16.15　zmore：查看gzip、zip、compress壓縮檔　193
16.16　bzip2：壓縮或解壓縮bzip2檔　194
16.17　bunzip2：壓縮或解壓縮bzip2檔　195
16.18　bzcat：解壓縮bzip2檔到標準輸出　195
16.19　bzcmp：比較bzip2壓縮檔　196
16.20　bzdiff：比較bzip2壓縮檔　196
16.21　bzgrep：在bzip2壓縮檔上搜索可能的規則運算式　197
16.22　bzip2recover：從損壞的bzip2檔中恢復資料　197
16.23　bzless：查看bzip2壓縮檔　197
16.24　bzmore：查看bzip2壓縮檔　198
16.25　compress：壓縮或解壓縮compress檔　198
16.26　uncompres：壓縮或解壓縮compress檔　199
16.27　znew：將.Z壓縮格式檔重新壓縮為.gz壓縮格式檔　200
16.28　xz：壓縮或解壓縮xz檔　200
16.29　xzcat：查看xz壓縮檔的內容　201
16.30　xzcmp：比較xz壓縮檔　201
16.31　xzdiff：比較xz壓縮檔　202
16.32　xzdec：解壓縮xz檔　202
16.33　xzgrep：在xz壓縮檔上搜索規則運算式　202
16.34　xzless：查看xz壓縮文字檔　203
16.35　xzmore：查看xz壓縮文字檔　203
16.36　tgz：將檔案壓縮為.tgz格式檔　203
16.37　gzexe：使用自身的壓縮版本重命名指定檔　203

第 17章　套裝軟體管理　205
17.1　rpm：RPM套裝軟體管理器　205
17.2　rpmargs：處理RPM套裝軟體　210
17.3　rpmbuild：構建RPM套裝軟體　210
17.4　rpmdiff：比較兩個套裝軟體之間的不同　211
17.5　rpmelfsym：在RPM套裝軟體中通過目的檔列出符號　212
17.6　rpmfile：在RPM套裝軟體中列出檔模式和類型　213
17.7　rpmlint：檢查rpm套裝軟體中的常見錯誤　213
17.8　rpm2cpio：從RPM套裝軟體中提取cpio歸檔　214

17.9　yum：YUM管理器 　214
17.10　yum-builddep：安裝建立指定的包所需要的RPM包　223
17.11　yum-complete-transaction：嘗試完成系統上不完整或中止的yum事物　224
17.12　yumdb：查詢和修改yum資料庫　225
17.13　yum-debug-dump：為yum創建調試問題的gzip壓縮檔　226
17.14　yum-debug-restore：借助yum-debug-dump創建的gzip壓縮檔進行還原　227
17.15　yumdownloader：從YUM軟體倉庫中下載RPM安裝包　227
17.16　yum-groups-manager：創建和編輯yum的組中繼資料　228
17.17　yum-config-manager：YUM配置管理　228

第 18章　磁碟分割　230
18.1　fdisk：分區表管理　230
18.2　parted：分區維護程式　236
18.3　cfdisk：基於磁片進行分區操作　238
18.4　partx：告訴內核關於磁片上分區的號碼　239
18.5　sfdisk：用於Linux的分區表管理　240
18.6　delpart：在Linux內核中刪除分區　241
18.7　partprobe：告知作業系統分區表更改　242

第 19章　檔案系統管理　243
19.1　mkfs：創建Linux檔案系統　243
19.2　mke2fs：創建ext2、ext3、ext4檔案系統　244
19.3　mkfs.ext4：創建ext4檔案系統　244
19.4　mkfs.ext3：創建ext3檔案系統　245
19.5　mkfs.ext2：創建ext2檔案系統　245
19.6　mkdosfs：創建MS-DOS檔案系統　245
19.7　mkfs.vfat：創建vfat檔案系統　246
19.8　mkfs.msdos：創建MS-DOS檔案系統　246
19.9　fdformat：低級格式化軟碟 　246
19.10　mount：掛載檔案系統　247
19.11　umount：卸載檔案系統　248
19.12　df：顯示檔案系統資訊　249
19.13　mountpoint：查看目錄是不是一個掛載點　251
19.14　e2label：顯示或更改檔案系統標籤　251
19.15　dumpe2fs：查看檔案系統信息　251
19.16　tune2fs：顯示和調整檔案系統參數　253
19.17　findfs：通過標籤或UUID查找檔案系統　255
19.18　blkid：顯示塊設備屬性　255
19.19　e2image：保存關鍵ext2、ext3、ext4檔案系統中繼資料　257
19.20　fsck：檢查和修復檔案系統　257
19.21　e2fsck：檢查 Linux ext2、ext3、ext4檔案系統　258
19.22　fsadm：在設備上調整或檢查檔案系統　259
19.23　mkswap：設置Linux交換分區　260
19.24　swapon：啟用交換分區或交換檔　261
19.25　swapoff：禁用交換分區或交換檔　261
19.26　volname：返回ISO 9660檔案系統的卷名　262

第 20章　磁片配額　263
20.1　quotacheck：創建、檢查和修復配額檔　263
20.2　edquota：編輯使用者磁片配額 　263
20.3　quotaon：啟用檔案系統磁片配額　265
20.4　quota：顯示磁片使用情況和限制　265
20.5　repquota：為檔案系統總結磁片配額　266
20.6　quotastats：查詢磁片配額統計資料　267
20.7　setquota：設置磁片配額　267
20.8　quotaoff：關閉檔案系統磁片配額　268
20.9　warnquota：發送郵件給超出配額的用戶　269
20.10　convertquota：從舊檔案格式轉換配額為新檔案格式　269

第 21章　LVM和RAID管理　270
21.1　pvcreate：創建物理卷　270
21.2　pvscan：列出找到的物理卷　272
21.3　pvdisplay：顯示物理卷的相關屬性　272
21.4　vgcreate：創建卷組　273
21.5　vgscan：查找所有的卷組　274
21.6　vgdisplay：顯示卷組的相關屬性 　274
21.7　vgreduce：從卷組中刪除未使用的物理卷 　275
21.8　vgextend：動態擴展卷組　275
21.9　lvcreate：創建邏輯卷　276
21.10　lvscan：列出所有卷組中的邏輯卷　276
21.11　lvdisplay：顯示邏輯卷的相關屬性　277
21.12　lvextend：擴展邏輯卷大小　277
21.13　resize2fs：檔案系統大小調整　278
21.14　lvremove：刪除邏輯卷　278
21.15　vgchange：更改卷組屬性　279
21.16　vgremove：刪除卷組　279
21.17　pvremove：刪除物理卷　280
21.18　pvchange：更改物理卷屬性 　280
21.19　pvck：檢查物理卷中繼資料　281
21.20　pvresize：調整一個卷組中的物理卷的大小　282
21.21　pvmove：移動物理盤區　282
21.22　pvs：輸出有關物理卷的報告資訊　283
21.23　vgcfgbackup：備份卷組描述符區域 　283
21.24　vgcfgrestore：還原卷組描述符區域 　284
21.25　vgchange：更改卷組屬性　284
21.26　vgconvert：轉換卷組中繼資料格式　285
21.27　vgexport：匯出卷組　286
21.28　vgimport：導入卷組　286
21.29　vgimportclone：導入並重命名複製的卷組　286
21.30　vgmerge：合併兩個卷組 　287
21.31　vgmknodes：重新創建卷組目錄和邏輯卷特殊檔　288
21.32　vgrename：重命名卷組名稱 　288
21.33　vgs：報告關於卷組的資訊　289
21.34　vgsplit：卷組拆分為兩個　289
21.35　lvchange：更改邏輯卷屬性 　290
21.36　lvmconf：LVM配置修改　291
21.37　lvmdiskscan：掃描可見LVM2所有設備 　291
21.38　lvmdump：轉儲LVM2有關的各種資訊　292
21.39　lvmetad：啟動LVM中繼資料快取記憶體守護進程　293
21.40　lvreduce：減小邏輯卷大小　293
21.41　lvrename：重命名邏輯卷 　294
21.42　lvresize：調整邏輯卷大小　294
21.43　lvs：報告有關邏輯卷的資訊　295
21.44　mdadm：管理Linux軟RAID　296

第 22章　GRUB　303
22.1　grub-md5-crypt：使用MD5格式加密口令　303
22.2　grub-install：在設備上安裝GRUB　303
22.3　grub：進入GRUB命令Shell　304
22.4　grub-crypt：對口令進行加密　306

第 23章　進程和服務管理　307
23.1　ps：報告當前進程的快照　307
23.2　top：顯示當前正在運行的進程　310
23.3　pgrep：按名稱和其他屬性查找進程　314
23.4　pidof：查找正在運行的進程的進程號　314
23.5　pstree：顯示正在運行的進程的進程樹　315
23.6　kill：終止進程　317
23.7　killall：按名稱殺死進程　318
23.8　pkill：按名稱和其他屬性殺死進程　319
23.9　timeout：在指定時間後仍在運行則殺死該進程　319
23.10　skill：發送一個信號或報告進程狀態　320
23.11　wait：等待指定的進程　320
23.12　fuser：顯示哪些進程使用指定的檔、通訊端或檔案系統　321
23.13　nice：以指定優先順序運行命令　322
23.14　renice：更改正在運行進程的優先順序　323
23.15　nohup：運行指定的命令不受掛起　323
23.16　pmap：報告進程的記憶體映射　324
23.17　lsof：列出打開的文件　326
23.18　ntsysv：配置服務在系統啟動時自動啟動或停止　328
23.19　chkconfig：為系統服務更新和查詢運行級別資訊　329
23.20　service：運行System V init腳本　330
23.21　bg：恢復在後臺暫停工作的作業　331
23.22　fg：將程式或命令放到前臺執行　332
23.23　jobs：列出作業　332
23.24　initctl：控制和管理init守護進程　333

第 24章　任務計畫　335
24.1　crontab：針對個人用戶維護crontab檔　335
24.2　at：在指定時間執行命令　336
24.3　atq：列出用戶等待執行的作業　337
24.4　atrm：刪除作業　337
24.5　atrun：稍後執行運行作業佇列　338
24.6　batch：當負荷平均下降到低於0.8時執行命令　338
24.7　anacron：定期運行命令　338
24.8　watch：定期執行一個程式　339

第 25章　備份與還原　340
25.1　mkisofs：創建ISO9660/Joliet/HFS檔案系統　340
25.2　isosize：輸出iso9660檔案系統的長度　342
25.3　dump：ext2/3/4檔案系統備份　342
25.4　restore：從dump備份中還原檔和檔案系統　344
25.5　cpio：存取歸檔包中的檔　346
25.6　dd：轉換和複製檔　348
25.7　wodim：將資料寫入光碟介質　349
25.8　cdrecord：將資料寫入CD光碟介質　351
25.9　dvdrecord：將資料寫入DVD光碟介質　351
25.10　cdrwtool：在CD-R、CD-RW和DVD-R設備上執行各種動作　351

第 26章　模組和內核管理　353
26.1　lsmod：顯示內核中模組的狀態　353
26.2　get_module：查看內核模組詳細資訊　354
26.3　modinfo：顯示內核模組資訊　355
26.4　insmod：插入模組到內核中　355
26.5　modprobe：在內核中添加和刪除模組　356
26.6　rmmod：在內核中刪除模組　358
26.7　depmod：生成modules.dep文件和映射文件　358
26.8　sysctl：在系統運行時配置內核參數　359
26.9　kexec：直接重啟進入一個新的內核　361
26.10　slabtop：即時顯示內核slab緩存資訊　362
26.11　dmesg：顯示或控制內核環形（ring）緩衝區　363
26.12　make：編輯內核或模組　365

第 27章　日誌管理　366
27.1　logwatch：系統日誌分析和報告　366
27.2　logger：在系統日誌中記錄相應條目　367
27.3　logsave：保存一個命令的輸出到日誌檔中　367
27.4　logresolve：在Apache日誌檔中解析IP位址為主機名稱　368

第 28章　硬體管理　369
28.1　lscpu：顯示有關CPU架構的資訊　369
28.2　nproc：顯示當前進程可用的CPU數目　370
28.3　chcpu：配置CPU 　370
28.4　cpuspeed：使用者空間的CPU頻率調節　371
28.5　free：顯示系統中的空閒和已用記憶體量　371
28.6　lspci：列出所有的PCI設備　373
28.7　setpci：配置PCI設備　376
28.8　lsscsi：列出SCSI設備及屬性　377
28.9　hdparm：顯示或設置硬碟參數　379
28.10　eject：彈出可移動介質　381
28.11　lsusb：列出USB設備　382
28.12　usb-devices：顯示USB設備的詳細資訊　384
28.13　lspcmcia：顯示擴展的PCMCIA調試資訊　385
28.14　pccardctl：PCMCIA卡控制工具　385
28.15　setserial：獲取和設置Linux串口資訊　386
28.16　lssubsys：列出包含指定子系統的層次結構 　387
28.17　lpinfo：顯示可用的設備或驅動程式　387
28.18　losetup：設置和控制迴圈設備　388
28.19　blockdev：從命令列調用塊設備讀寫控制　389
28.20　dmidecode：DMI表解碼器　390
28.21　systool：按匯流排、類和拓撲查看系統設備資訊　396
28.22　mev：報告滑鼠事件 　397
28.23　loadkeys：載入鍵盤轉換表　397
28.24　dumpkeys：轉儲鍵盤轉換表　398
28.25　minicom：友好的串口通信程式　398
28.26　arch：顯示電腦主機的體系結構　399
28.27　sync：將緩衝檔寫到硬碟中　399

第 29章　SELinux管理　400
29.1　sestatus：顯示SELinux狀態　400
29.2　getenforce：顯示當前SELinux的應用模式　401
29.3　setenforce：修改SELinux的應用模式　401
29.4　getfattr：獲取檔案系統物件的擴展屬性　401
29.5　chcon：修改檔SELinux安全上下文　402
29.6　matchpathcon：查看檔默認安全上下文　403
29.7　fixfiles：修復安全上下文　403
29.8　restorecon：修復檔默認的SELinux安全上下文　404
29.9　seinfo：顯示SELinux策略的元件有關的資訊　405
29.10　sesearch：在SELInux策略中搜索規則　406
29.11　getsebool：查看SELinux布林值　407
29.12　setsebool：修改SELinux布林值　408
29.13　semodule：管理SELinux策略模組　409

第30章 審計系統　411
30.1　auditctl：控制內核的審計系統　411
30.2　aureport：生成審計資訊報表　413
30.3　ausearch：搜索審計記錄　416
30.4　autrace：跟蹤指定進程　417
30.5　audit-viewer：查看和總結審計事件的圖形工具　417

第31章　設備管理　418
31.1　udevadm info：查詢udev資料庫中的設備資訊　418
31.2　mknod：創建塊設備和字元設備檔 　421
31.3　MAKEDEV：創建/dev中的設備　422
31.4　lsblk：列出塊設備資訊　423

第32章　性能監控　426
32.1　sar：收集、報告或保存系統活動資訊　426
32.2　iostat：報告CPU統計資料和設備、分區輸入/輸出資訊　429
32.3　iotop：進行I/O監控　430
32.4　mpstat：報告CPU相關的統計資料　432
32.5　vmstat：報告虛擬記憶體統計　433
32.6　tload：載入顯示系統平均負載　435
32.7　time：給出資源使用的時間　436
32.8　uptime：顯示系統已經運行的時間　436
32.9　ipcs：提供IPC設施資訊　437
32.10　ipcrm：刪除訊息佇列、信號量集或共用記憶體ID　438
32.11　lslk：列出本地鎖　439

第33章　X Window　441
33.1　xhost：X伺服器的存取控制程式　441
33.2　xinit：X Window系統初始化　441
33.3　xlsclients：在顯示器中列出正在運行的用戶端應用程式 　442
33.4　xlsfonts：顯示X伺服器字體清單　442
33.5　resize：設置xterm視窗大小　443
33.6　startx：初始化一個X會話　444
33.7　screen：VT100/ANSI終端模擬螢幕管理　444
33.8　xset：顯示或設置顯示器的使用者首 選項　446
33.9　xauth：X許可權檔實用工具　446

第34章　列印和傳真　448
34.1　lpr：列印檔案　448
34.2　lpq：顯示列印佇列狀態　448
34.3　lprm：取消列印工作　449
34.4　lpstat：顯示cups狀態資訊　449
34.5　cupsaccept：接受作業發送到目的地　450
34.6　cupsreject：拒絕作業發送到目的地　451
34.7　cupsenable：啟動印表機和類　451
34.8　cupsdisable：停止印表機和類 　451
34.9　cancel：取消列印　452
34.10　lp：列印檔案　452
34.11　lpadmin：配置cups印表機和類　453
34.12　efax：以1、2或2.0級傳真數據機發送/接收傳真　454

第35章　終端　456
35.1　tty：顯示連接到當前標準輸入的終端設備檔案名　456
35.2　consoletype：顯示連接到標準輸入的控制台類型 　456
35.3　fgconsole：顯示活動的虛擬終端數量　456
35.4　mingetty：用於控制台的精簡版getty　457
35.5　vlock：鎖定虛擬控制台　458
35.6　stty：輸出或修改終端參數　458
35.7　tset：終端初始化　459
35.8　open：啟用虛擬終端　459
35.9　reset：終端初始化　460
35.10　securetty：添加tty到/etc/securetty文件　460
35.11　tput：初始化一個終端或查詢terminfo資料庫　461

第36章　密碼和證書管理　462
36.1　pwdhash：密碼雜湊生成器　462
36.2　mkpasswd：生成應用於使用者的新密碼　462
36.3　keytool：金鑰和證書管理工具　463
36.4　certutil：證書伺服器管理工具 　464
36.5　vncpasswd：創建或更改VNC登錄密碼　465
36.6　ssh-keygen：創建SSH金鑰　465
36.7　htpasswd：為基本驗證管理用戶文件　467
36.8　htdigest：管理用於摘要認證的用戶文件　468
36.9　ntp-keygen：生成NTP主機金鑰　468
36.10　slappasswd：設置LDAP管理員密碼　470
36.11　rndc-confgen：金鑰生成工具 　471
36.12　openssl：OpenSSL命令列工具　472

第37章　Linux系統故障排錯　474
37.1　mkbootdisk：創建用於運行系統的獨立啟動軟碟　474
37.2　chroot：切換根目錄環境 　474
37.3　badblocks：搜索設備的壞塊　475
37.4　mkinitrd：創建要載入ramdisk的映射檔　476
37.5　switch_root：切換到另一個作為掛載樹的根的檔案系統　476
37.6　mkdumprd：為內核轉儲崩潰恢復創建初始ramdisk映射　476

第38章　網路命令　478
38.1　traceroute：顯示跟蹤到網路主機的路由資料包　478
38.2　mii-tool：查看、操縱網路介面狀態　479
38.3　ifconfig：顯示和配置網路介面　480
38.4　ifdown：關閉網路介面　481
38.5　ifup：開啟網路介面　481
38.6　ping：測試與目的電腦之間的連通性　482
38.7　netstat：顯示網路連接、路由表、介面統計、偽裝連接和組播成員　483
38.8　arp：操縱系統ARP緩存　484
38.9　rpcinfo：顯示使用portmap註冊的程式資訊　485
38.10　ip：顯示和操縱路由、設備、策略路由和隧道　487
38.11　tracepath：跟蹤到目的網路主機的路徑　490
38.12　ifcfg：進行IP位址管理　491
38.13　setup：文字模式系統組態工具　491
38.14　arping：發送ARP REQUEST到相鄰主機　492
38.15　ss：獲取通訊端統計資訊　493
38.16　ipcalc：執行IP位址的簡單操作　496
38.17　arpwatch：為乙太網/IP位址配對保持跟蹤　497
38.18　arpaname：IP位址轉換為對應的ARPA名稱　497
38.19　route：添加、刪除和查看IP路由表　498
38.20　nntptest：互動式NNTP測試程式　499
38.21　rpcbind：通用位址到RPC程式號映射器　500
38.22　usernetctl：允許使用者操縱網路介面　501
38.23　iwconfig：配置無線網路介面　501

第39章　網路安全　504
39.1　rtacct：網路統計工具　504
39.2　nmap：報告遠端主機特徵　504
39.3　tcpdump：實現網路資料獲取分析　510
39.4　iptstate：顯示IP表狀態表條目　512
39.5　nstat：監視內核SNMP計數器和網路介面統計資料　514
39.6　iptraf：互動的IP網路監控　515
39.7　lnstat：查看網路統計資訊　516
39.8　nc：進行任意的TCP和UDP連接和監聽　518
39.9　mtr：實現traceroute和ping程式的網路診斷工具 　519

第40章　網路用戶端端　520
40.1　elinks：字元模式的Web流覽器　520
40.2　wget：從Web網站下載檔案　521
40.3　curl：傳輸URL　522
40.4　lynx：通用分散式資訊的萬維網流覽器　525
40.5　lftp：實現檔案傳輸　528
40.6　lftpget：使用lftp下載檔案　530
40.7　telnet：通過TELNET協定和遠端主機進行通信　530
40.8　tftp：TFTP用戶端　531
40.9　ftp：ARPANET檔案傳輸程式　532
40.10　mutt：Mutt郵件使用者代理　534
40.11　mailx：發送和接收郵件　535
40.12　mail：發送和接收郵件　537
40.13　vncviewer：連接VNC伺服器　537
40.14　smbclient：顯示和連接Samba共用目錄　538
40.15　smbget：下載Samba共用資源　541
40.16　svn： Subversion命令列用戶端程式　542
40.17　ssh：遠端登入程式　547
40.18　scp：安全遠端檔複製程式　548
40.19　sftp：安全的檔案傳輸程式　549
40.20　mount.nfs4：掛載NFS v4檔案系統 　551
40.1　mount.nfs：掛載NFS檔案系統 　551
40.22　umount.nfs：卸載NFS檔案系統　552
40.23　dhclient：配置DHCP用戶端　552
40.24　ntpdate：通過NTP伺服器來設置日期和時間　553

第41章　MySQL資料庫　554
41.1　mysqld_safe：MySQL伺服器啟動腳本　554
41.2　mysql_install_db：初始化MySQL資料目錄 　554
41.3　mysqlshow：顯示MySQL資料庫結構　555
41.4　mysqladmin：管理MySQL伺服器　557
41.5　myisamchk：檢查和修復MyISAM表　559
41.6　mysql：MySQL命令列工具　560
41.7　mysqlimport：實現資料導入　562
41.8　mysqlcheck：檢查和修復MyISAM表　563
41.9　mysqlbinlog：查看二進位日誌檔　564
41.10　mysqldumpslow：顯示慢查詢日誌檔摘要　566
41.11　mysqldump：備份資料庫　567
41.12　mysqlhotcopy：備份資料庫　568

第42章　PostgreSQL資料庫　570
42.1　initdb：初始化PostgreSQL資料庫　570
42.2　pg_ctl：控制PostgreSQL服務　572
42.3　psql：PostgreSQL互動式用戶端工具　573
42.4　createdb：創建PostgreSQL資料庫　576
42.5　dropdb：刪除PostgreSQL資料庫　577
42.6　vacuumdb：清理並優化PostgreSQL資料庫　577
42.7　createuser：創建PostgreSQL用戶　578
42.8　dropuser：刪除PostgreSQL用戶　579
42.9　pg_dump：備份資料庫　580
42.10　pg_dumpall：備份所有資料庫　581
42.11　pg_restore：恢復資料庫　582

第43章　iptables和arptables防火牆　584
43.1　iptables-save：保存iptables規則　584
43.2　iptables-restore：恢復iptables規則　584
43.3　iptables：IPv4資料包過濾和NAT管理工具　585
43.4　arptables-save：保存ARP表　591
43.5　arptables-restore：還原ARP表　591
43.6　arptables：ARP資料包過濾管理工具　592

第44章　PPPoE配置　595
44.1　pppoe-setup：配置PPPoE用戶端　595
44.2　pppoe-connect：管理PPPoE鏈路　597
44.3　pppoe-start：啟動PPPoE鏈路　597
44.4　pppoe-stop：關閉PPPoE鏈路　598
44.5　pppoe-status：報告PPPoE鏈路的狀態　598
44.6　pppoe-sniff：為非標準的PPPoE幀檢查網路　598
44.7　pppoe-server：用戶空間的PPPoE伺服器　598
44.8　pppoe-relay：使用者空間的PPPoE中繼代理　599
44.9　pppstats：顯示PPP連接狀態　600

第45章　伺服器配置　601
45.1　ssh-agent：存儲用於公開金鑰驗證的私密金鑰　601
45.2　ssh-add：添加RSA或DSA身份的認證代理　601
45.3　ssh-keyscan：收集主機公開金鑰　602
45.4　sshd：運行sshd守護進程　603

45.5　vncserver：管理VNC伺服器　603
45.6　exportfs：匯出NFS伺服器上的共用目錄　605
45.7　showmount：查看NFS共用目錄資訊　606
45.8　nfsstat：顯示NFS活動統計資訊　606
45.9　mountstats：顯示NFS用戶端統計資訊　607
45.10　nfsiostat：顯示NFS客戶機掛載統計資訊　609
45.11　testparm：檢查smb.conf設定檔的內部正確性　609
45.12　smbpasswd：創建Samba帳戶　610
45.13　smbstatus：顯示當前Samba連接報告　610
45.14　pdbedit：管理Samba使用者資料庫　611
45.15　smbtree：基於文本進行SMB網路流覽　615
45.16　nmblookup：通過TCP/IP用戶端來查找NetBIOS名稱　616
45.17　dhcpd：運行DHCP伺服器　617
45.18　dhcrelay：提供中繼DHCP和BOOTP請求　618
45.19　rndc：控制DNS伺服器操作　619

45.20　named-checkconf：named設定檔語法檢查　621
45.21　named-checkzone：區域檔有效性檢查和轉換　621
45.22　named-compilezone：轉儲區域內容到指定檔　622

45.23　host：執行DNS查找進行功能變數名稱解析　623
45.24　nslookup：以互動式和非互動式方式查詢功能變數名稱　624
45.25　dig：DNS查詢　626
45.26　jwhois：在命令列上為物件搜索Whois伺服器　628
45.27　whois：在命令列上為物件搜索Whois伺服器　629
45.28　dnsdomainname：顯示DNS功能變數名稱　629
45.29　nsupdate：進行動態DNS更新　630
45.30　apachectl：控制Apache伺服器　631
45.31　httpd：運行Apache超文字傳輸協定伺服器　634
45.32　ab：Apache HTTP伺服器基準測試　635
45.33　postalias：維護Postfix別名資料庫　636
45.34　postconf：Postfix配置工具　636
45.35　svnadmin：管理SVN版本庫　638
45.36　svnserve：啟動SVN服務　639
45.37　nisdomainname：顯示或設置NIS功能變數名稱　640
45.38　domainname：顯示或設置系統的NIS/YP功能變數名稱 　640
45.39　ypdomainname：顯示或設置NIS/YP功能變數名稱　641
45.40　ypinit：創建NIS資料庫 　642
45.41　yptest：調用不同的NIS函數來測試NIS配置　643
45.42　ypwhich：列出NIS伺服器的名稱及昵稱轉換表　644
45.43　ypcat：指定映射名顯示所有鍵的值　645
45.44　ypmatch：顯示NIS映射中指定鍵的值　646
45.45　yppasswd：更改使用者的NIS密碼、Shell和通用資訊　647
45.46　ypchsh：更改用戶的登錄Shell類型　　 　648
45.47　ypset：綁定ypbind到特定的NIS伺服器　648
45.48　yppoll：顯示當前伺服器上使用的NIS映射的順序號（標識號）　649
45.49　ypxfr：同步設置　649
45.50　ypserv：運行ypserv守護進程　650
45.51　ypbind：進行NIS綁定處理　650

45.52　ntpstat：顯示網路時間同步狀態　651
45.53　ntpq：查看NTP服務同步狀態　651
45.54　ntptime：讀取核心程式的時間變數　654
45.55　ntpdc：詢和更改當前ntpd守護進程的狀態　654
45.56　makemap：為Sendmail創建資料庫映射　657
45.57　mailq：顯示郵件佇列　657
45.58　mailstats：顯示郵件統計資訊　658
45.59　fetchmail：郵件檢索和轉發工具　658
45.60　sendmail：電子郵件傳輸代理　660
45.61　zebra：運行zebra守護進程　661
45.62　squid：運行Squid伺服器　662
45.63　squidclient：從緩存中檢索和清除URL　663
45.64　slaptest：檢查OpenLDAP設定檔　663
45.65　ldapadd：添加LDAP條目　664
45.66　ldapsearch：查詢LDAP資料資訊　666
45.67　slapcat：LDAP數據匯出成LDIF　671
45.68　ldapmodify：修改LDAP條目　673
45.69　ldapdelete：刪除LDAP條目　674
45.70　slapindex：在SLAPD資料庫中重新索引條目　675
45.71　slapschema：資料庫模式檢查實用程式　676
45.72　slapauth：檢查slapd行為映射身份驗證和授權　676
45.73　slapadd：添加LDIF格式的條目到SLAPD資料庫　677
45.74　slapacl：檢查訪問屬性的清單　678
45.75　slaptest：檢查slapd.conf設定檔的一致性　678
45.76　slapd：運行slapd守護進程　679

第46章　其他命令　680
46.1　mkfontdir：創建X字體檔的索引　680
46.2　dumpiso：轉儲IEEE 1394同步通道的資料包　680
46.3　iconv：轉換檔編碼　681
46.4　hash：顯示和刪除雜湊表　681
46.5　lsb_release：顯示LSB和特定版本的相關資訊　682
46.6　locale：獲取特定語言環境　683
46.7　nm：從目的檔中列出符號　685
46.8　rmt：遠端磁帶傳輸協定模組　685
46.9　lscgroup：列出所有的cgroups　686
46.10　cgclear：卸載cgroup檔案系統　686
46.11　cachefilesd：運行CacheFiles使用者空間管理守護進程 　687
46.12　uuid：通用唯 一識別字命令列工具　687
46.13　uuidd：運行UUID生成守護進程　688
46.14　ar：創建、修改並從歸檔中提取檔　688
46.15　arpd：運行arp守護進程　690
46.16　automount：管理autofs掛載點　690
46.17　col：從輸入中過濾控制字元　691
46.18　diffstat：顯示diff輸出的統計資訊　691
46.19　dircolors：輸出用來設置LS_COLORS的環境變數　693
46.20　ldd：顯示共用庫的依賴關係　693
46.21　ldconfig：配置運行時綁定動態連結程式　694
46.22　hostid：顯示當前主機的數位識別碼符　695
46.23　uname：顯示電腦及作業系統的相關資訊　695
46.24　hostname：顯示或修改電腦主機名稱　696
46.25　echo：在顯示器上顯示文字　697
46.26　yes：重複輸出一行指定的字串，或重複輸出y　698
46.27　printf：格式和列印資料　698
46.28　mesg：允許或拒絕寫消息　699
46.29　wall：對全部已登錄使用者發送資訊　699
46.30　write：向使用者發送消息　699
46.31　clear：清除電腦螢幕資訊　700
46.32　type：顯示命令的類型　700
46.33　bind：顯示或設置readline鍵和函數綁定　701
46.34　pjtoppm：轉換HP PaintJet檔為PPM圖像 　702
46.35　qrttoppm：QRT檔轉換輸出為PPM圖像　702
46.36　fiascotopnm：轉換壓縮FIASCO圖像到PGM或PPM 　702

```
