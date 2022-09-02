
20220828

| CMD | NAME | OPTION | NOTE |  
| :----| ----: | :----: | :---- |  
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
|  |  |  |  |  
|  |  |  |  |  


|  |  |  |  |  
| :----| ----: | :----: | :---- |  
| cp /etc/passwd /home/test | 將passwd檔案複製到~ |  |  |  
| vim +/login passwd | 高亮login,瀏覽passwd檔案 |  |  |  
| 編輯模式 |  |  |  |  
| :----| ----: | :----: | :---- |  
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
| /關鍵詞 | 搜索關鍵詞 |  |  |  
| N/n | 在搜索結果中切換上/下一個結果 |  |  |  
| :nohl | no highlight 取消高亮 |  |  |  
| :s/關鍵詞/替換的內容 | replace |  |  |  
| :s/關鍵詞/替換的內容/g | replace all |  |  |  
|  |  |  |  |  
|  |  |  |  |  
|  |  |  |  |  


