x444炸群工具 使用說明
====  
## 建立機器人及設定必要選項
首先你需要先去設定把"開發者模式"打開  
>左下角齒輪➤進階➤開發者模式  

接下來你需要去[這裡](https://discord.com/developers/applications)創建一個機器人  
然後到BOT的選項把這三個選項都給它打勾
>PRESENCE INTENT  
SERVER MEMBERS INTENT  
MESSAGE CONTENT INTENT  

打勾之後往上滑，按下Reset Token，然後把它顯示出來的Token複製下來
## 炸群檔案設定
先解壓縮檔案
接下來打開 config.json 把token複製到第二行的 "這裡請幫我填上機器人token"   
你可以自己自訂你想要創建的頻道名稱、身分組名稱及刷頻的文字  
### config.json預覽
```json
{
    "token": "這裡請幫我填上機器人token",
    "proxy": false,
    "nuke": {
        "channels_name": [
            "在這裡新增自訂的頻道名稱",
            "執行的時候會創建隨機的頻道",
            "如果要固定一種名稱的話",
            "就把其他三個刪掉，然後把自訂文字第一串的逗號刪掉"
        ],
        "roles_name": [
            "隨機身分組名稱",
            "創建時會三個隨機創建",
            "想固定只創建一個名稱的話請按照上面的步驟"
        ],
        "messages_content": [
            "隨機刷頻字串",
            "同上",
            "建議tag everyone",
            "機器人的tag會無視群組身分組設定"
        ]
    }
}
```   
## 實戰
接下來就是實戰了，你可以參考我這部影片的操作 https://youtu.be/taK1yXe8oJU  
先邀請機器人到目標群組，並給它管理員權限   
然後複製群組的ID，貼到x444的視窗中然後按下Enter  
然後他就會顯示它的功能表，請用相對應的數字來選擇使用的功能  
下列是功能表的預覽，中文及英文
| 代號 | 功能 | 代號 | 功能 | 代號 | 功能 |
|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|
|  1  | Ban Members |  5  | Create Roles | 9 | Spam Channels |
|  2  | Kick Members |  6  | Delete Channels | 10 | Check Updates |
|  3  | Prune Memnbers | 7 | Delete Roles | 11 | Credits |
|  4  | Create Channels | 8 | Delete Emoji | 12 | Exit |

| 代號 | 功能 | 代號 | 功能 | 代號 | 功能 |
|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|
|  1  | 停權所有成員 |  5  | 創建身分組 | 9 | 刷頻(不要太多，不然會被限速) |
|  2  | 踢出所有成員 |  6  | 刪除所有頻道 | 10 | 檢查更新 |
|  3  | 踢出所有不活躍成員 | 7 | 刪除所有身分組 | 11 | 製作團隊 |
|  4  | 創建文字&語音頻道 | 8 | 刪除所有Emoji | 12 | 退出程序 |
