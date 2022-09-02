
20220828

| CMD | NAME | OPTION | NOTE |  
| :---- | ----: | :----: | :---- |  
| mkdir | 創建資料夾 | mkdir 目錄名 |  |  
| touch | 創建資料夾/檔案 | touch 檔名 |  |  
| cp | 複製資料夾/檔案 | cp 檔名 路徑 |  |  
| mv | 移動資料夾/檔案 | mv 原路徑 新路徑 | 重新命名 | 
| rm | 移除檔案 | rm 路徑/文件名 | -f force強制，刪除不經確認 |  
| rm | 移除資料夾 | rm 文件 -rf | |  
| cat | 檢視檔案 | cat 路徑 | |  
| cat | 合併檔案 | cat 路徑1 路徑2 > 新檔案路徑 | |   
| df -h | 磁碟空間使用 |  |  |  
| free | 可使用磁碟空間 | -m以mb為單位 -g以gb為單位 |  |  
| head | 查看檔案的前10行 | -Number 指定前N行 |  |  
| tail | 查看檔案的末10行 | -Number 指定後N行 |  |  
| less | 以一頁為範圍查看檔案 |  |  |  
| wc | 統計檔案內容信息 | wc 路徑 -l表示行數 -w單詞數 -c表示bytes數 |  |  
| date | 輸出時間訊息 | date +%F 輸出形式年-月-日 date "%Y-%m-%d" |  |  
| cal | 輸出當前月份的日曆 | cal -Number |  |  
| hostname | 輸出主機名稱 | -f 全域名 |  |  
| id |  |  |  |  
| du | 查看目錄的真實大小 | du 路徑 -s只顯示匯總的大小 -h可讀 |  |  
| find | 查找文件 | find 路徑 檔名 | -name按照文件名稱 -type按照檔案類型(f文件 or d目錄) |  
| service | 服務 | service 服務名 start/stop/restart | service httpd start |  
| ps |  | ps -e列出全部的進程 -f顯示全部的列 | ps -ef|qrep httpd |  
| kill |  | kill 進程名稱 |  |  
| killall |  | killall 進程名稱 |  |  
| ifconfig | 獲取網卡信息 |  |  |  
| reboot | 重新啟動 |  |  |  
| shutdown | 關機 |  | shutdown -h 15:30 |  
| uptime | 輸出計算機的運行時長 |  |  |  
| netstat | 查看網路連接狀態 |　-t列出tcp協議 -n列出ip地址 -l過濾出state列中，值為listen的連接 -p顯示進程的pid和進程名稱  | netstat -tnlp |  
| man | 命令手冊 |  | man cp |  
| vim | 開啟檔案 | vim 路徑 | 可以開啟未存在檔案 |  
| vim |  | vim +數字 路徑 | 打開檔案,移動到指定行 |  
| vim |  | vim +/關鍵詞 路徑 | 打開檔案，高亮關鍵詞 |  
| ls | 列出資料夾檔案列表 |  |  |  
| ll | 列出檔案詳細 | ll -a | 列出隱藏檔 |  
| | |  |  |  
| | |  |  |  


|  |  |  |  |  
| :---- | ----: | :----: | :---- |  
| cp /etc/passwd /home/test | 將passwd檔案複製到~ |  |  |  
| vim +/login passwd | 高亮login,瀏覽passwd檔案 |  |  | 

| 編輯模式 |  |  |  |  
| :---- | ----: | :----: | :---- |  
| shift + 6 | 移動到行首 | 6 = ^ |  |  
| shift + 4 | 移動到行尾 | 4 = $ |  |  
| gg | 移動到首行 |  |  |  
| G | 移動到末行 |  |  |  
| 10G | 移動到第10行 |  |  |  
| 10上 | 往上移10行 |  |  |  
| 10下 | 往下移10行 |  |  |  
| 10左 | 往左移10字 |  |  |  
| 10右 | 往右移10字 |  |  |  
| ctrl + b | 往上一頁 |  |  |  
| ctrl + f | 往下一頁 |  |  |  
| yy | 複製光標所在行 |  |  |  
| 3yy | 複製光標所在行 +往下2行 |  |  |  
| p | 貼上複製行 |  |  |  
| dd | 剪下光標所在行 |  |  |  
| 3dd |  |  |  |  
| D | 剪下光標所在行,下一行不上移 |  |  |  
| :u | 恢復上一個動作 | ctrl + z |  |  
| u | 恢復上一個動作 |  |  |  
| ctrl + r | (撤銷)恢復上一個動作 |  |  |  
| :w | 保存檔案 |  |  |  
| :w 路徑 | 另存檔案 |  |  |  
| :wq | 保存檔案，並退出 |  |  |  
| :x | 保存檔案，並退出 | 未修改的情況下，不會更改檔案編輯時間 |  |  
| /關鍵詞 | 搜索關鍵詞 |  |  |  
| N/n | 在搜索結果中切換上/下一個結果 |  |  |  
| :nohl | no highlight 取消高亮 |  |  |  
| :s/關鍵詞/替換的內容 | replace |  |  |  
| :s/關鍵詞/替換的內容/g | replace all |  |  |  
|  |  |  |  |  
| ln -s | 創造自定義命令捷徑 |  |  |  
|  |  |  |  |  
|  |  |  |  |  

| Vim 的配置 |  |   | |  
| :----| ----: | :----: | :---- |  
|  本地配置文件 ~/.vimrc  |  
|  全局配置文件 /etc/vimrc |  
| set nu | 顯示行號 |  |  
|  映射配置 |  
| cat ~/.vashrc | 檢視映射配置 |  |  |  
| vim ~/.vashrc |  編輯映射配置 |  |  |  
| alias cls='clear' | 用cls觸發clear命令 |  |  |  

| 重要文件 |  |  |  |  
| :----| ----: | :----: | :---- |  
| /etc/passwd | 存儲用戶的關鍵信息 |  |  |  
| /etc/group | 存儲用戶組的關鍵信息 |  |  |  
| /etc/shadow | 存儲用戶的密碼信息 |  |  |  
|  |  |  |  |  
| 用戶管理 |  |  |  |  
| useradd |  | -g指定用戶的用戶主組,值可以是用戶組的id,也可以是組名 |  |  
| useradd | -G指定用戶的用戶附加組,值可以是用戶組的id,也可以是組名 |  |  |  
| useradd | | -u uid,用戶的id(用戶的識別符),系統會從500之後按順序分配uid, -u 可以自定義 |  |  
| usermod | 用戶修改 |  | usermod -g 1003 iG 1003 lisi |  
| passwd | 修改用戶密碼 | passwd 用戶名 -> 新密碼 |  |  
| userdel | 刪除用戶 | userdel 用戶名 |  |  
| groupadd | 用戶組添加 | groupadd -g 1003 用戶名 |  |  
| groupdel | 刪除用戶組 |  |  |  
|  |  |  |  |  
|  |  |  |  |  
|  |  |  |  |  

| 網路設置 |  |  |  |  
| :----| ----: | :----: | :---- |  
| ls /etc/sysconfig/network-scripts |  |  |  |  
| cat /etc/sysconfig/network-scripts/ifcfg-enp0s3 |  |  |  |  
|  | ONBOOT | 使否開機啟動 |  |  
|  | BOOTPROTO | ip地址分配方式,DHCP表示動態主機分配協議 |  |  
|  | HWADDR | 硬件地址,MAC地址 |  |  
| 重啟網卡 |  |  |  |  
| service network restart |  |  |  |  
| ifdown | 停止網卡 | ifdown 網卡名 |  |  
| ifup | 啟用網卡 | ifup 網卡名 |  |  
| ls /etc/init.d/ |  |  |  |  
| /etc/init.d/network restart |  |  |  |  
|  |  |  |  |  
|  |  |  |  |  
|  |  |  |  |  
|  |  |  |  |  
|  |  |  |  |  
|  |  |  |  |  




