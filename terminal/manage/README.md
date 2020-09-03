* [获取日志清单](terminal/manage/getDevLog)
* [浏览文件目录](terminal/manage/readFile)
* [获取数据库](terminal/manage/getDB)
* [升级APP](terminal/manage/upgradeApp)
* [升级HTML](terminal/manage/upgradeHtml)
* [退出播放](terminal/manage/quitPlay)
* [重启APP](terminal/manage/relaunchApp)
* [退出APP](terminal/manage/quitApp)
* [截屏](terminal/manage/screenshot)
* [查看APP在前台](terminal/manage/isAppForeground)
* [查看节目播放](terminal/manage/isProgramRunning)


## 使用

### API说明

请求地址 = 终端的IP地址 + API名称

|API名称|请求类型|支持跨域|dataType|contentType|支持框架|
|--|--|--|--|--|--|
|command/execute|POST|Y|json|application/json|1.axios 2.jquery的ajax|


### 入参

|名称|编码|类型|必须|默认值|说明|
|--|--|--|--|--|--|
|命令|method|string|Y|cmd||
|是否需要通知|needNotify|boolean|N|false|需要返回数据时，必须填写true。默认为false|
|数据|data|object|N|无||

### 出参

|名称|编码|类型|必须|默认值|说明|
|--|--|--|--|--|--|
|返回码|code|init|Y|无|0代表请求成功|
|数据|data|object|N|false|有返回数据时有该字段|