# Facebook Messenger Practice
這個 Repo 是參照 [這個教學](http://animabeautifullife.blogspot.com/2016/06/facebook-messenger-api.html) 的練習
#### 建立粉絲專頁
因為 Bot 就是一個機器人來做自動回覆以及服務，粉絲專頁當作機器人的名字也是相當合理呢。

#### 在 GitHub 建立一個 Repo
也就是現在這個 Repo
```
https://github.com/sprewell20051116/facebookMessengerBot.git
```

#### Git Clone Facebook sample
將 Facebook 的 Sample `git clone` 下來
```sh
$ git clone  https://github.com/fbsamples/messenger-platform-samples.git
```
把自己的 GitHub repo 加入這個 Git remote 中，就可以把 facebook sample push 到自己的 GitHub 了 (當然你也可以直接 `fork` 他)
```sh
$ git add remote GitHub https://github.com/sprewell20051116/facebookMessengerBot.git
$ git push GitHub
```
#### 建立 Cloud9 Server
由 [Facebook Messenger 聊天機器人 API 環境建置 教學](http://animabeautifullife.blogspot.com/2016/06/facebook-messenger-api.html) 推薦，可以快速建置 NodeJS server, 並且提供 https 服務，可說是讓我這個網路開發超新手感到相當的蘇胡呢。Cloud9 的免費服務可以讓我們快速的驗證 Facebook messenger，不過唯有付費方案才有常駐服務。
詳細建立方式也請參照 [Facebook Messenger 聊天機器人 API 環境建置 教學](http://animabeautifullife.blogspot.com/2016/06/facebook-messenger-api.html)  這篇教學

#### 設定 Global Variable
設定 `./node/config/default.json` 中的各項參數，其中 `appSecret`、`pageAccessToken` 都可以在 facebook developers 主控台中找到。

```json
{
    "appSecret": "OOO",
    "pageAccessToken": "OOOOO",
    "validationToken": "GigigunCloud9",
    "serverURL": "https://messenger-gigigun1116.c9users.io/webhook"
}
```




#### ref:
- [Facebook Messenger 聊天機器人 API 環境建置 教學](http://animabeautifullife.blogspot.com/2016/06/facebook-messenger-api.html)
- [Facebook Messenger Quick Start](https://developers.facebook.com/docs/messenger-platform/getting-started/quick-start)
- [Cloud9](https://c9.io/)
