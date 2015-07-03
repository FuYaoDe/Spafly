# Spafly
Spafly 是一個簡單的 Bash/Applescript 可以使用 command line 在 Mac 上操控 [Spotify](https://www.spotify.com)，搭配排程 + crontab 讓您每天早上起床就像泡 SPA 一樣。

## Installation and usage
1. 下載 Spafly.zip 或是 clone 這個倉庫
    ````
    $ git clone 
    ````

2. 解壓縮後確保spafly是可執行的文件
    ````
    $ cd spafly
    $ chmod +x spafly
    ````

3. 把Spafly複製到方便的位置，然後設定PATH環境變數，或是直接
    ````
    $ sudo cp ./spafly/spafly /usr/bin/spafly
    ````

4. 完成了～ 你現在能試試看使用 spafly 播放音樂了
    ````
    $ spafly "spotify:user:spotifytaiwan:playlist:6rnBixkR4lXh2djtI6esk6"
    ````
    總覽
    ````
    spafly [-m <音量 1-100 > ] [-s] 音樂的分享網址
    ````
    音樂的分享網址能複製播放連結或Spotify URL

    ![音樂分享網址](https://github.com/FuYaoDe/Spafly/blob/master/url_example.png?raw=true)

    選項
    ````
    -m <音量 1-100> - 能調整最大的音量範圍為 1~100 , 如果沒設定預設是 80
    -s - 讓音樂淡入，讓你像在泡SPA一樣
    ````
    範例
    ````
    讓音樂淡入，且最大音量為 50
    spafly -m 50 -s "spotify:user:spotifytaiwan:playlist:6rnBixkR4lXh2djtI6esk6"

    讓音樂淡入，音量使用預設值 80
    spafly -s "https://open.spotify.com/user/spotifytaiwan/playlist/6rnBixkR4lXh2djtI6esk6"
    
    直接播放該音樂，音量使用預設值 80
    spafly "https://open.spotify.com/user/spotifytaiwan/playlist/6rnBixkR4lXh2djtI6esk6"
    ````

##特別感謝
* [hnarayanan](https://github.com/hnarayanan)
