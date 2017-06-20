# syncPlaylist
Sync playlist between WY and QQ.

## platform
1. Windows
2. MacOS
3. Linux

---------------
## requirement
1. beautifulsoup4
2. requests
3. selenium

---------------
## Usage

### Step 1: Download the driver
Download phantomjs driver [here](http://phantomjs.org/download.html). Unzip it. So you can find driver is `[download_path]/phantomjs-X.X.X/bin/phantomjs`. For example: `D:/Downloads/phantomjs-2.1.1-windows/bin/phantomjs`(windows) or `/Users/denon/Downloads/phantomjs-2.1.1-macosx/bin/phantomjs` (Linux or Mac OS)


### Setp 2: set driver path and input config
* write the driver absolute path in `settings.py`.`phantomjs_driver_path`
input account config



* If you choose WY to QQ:
1. add your qq account and password in `config.json`[qq_account, qq_password]
2. copy 163 playlist url in `config.json`[wy_playlist_url]
3. input qq playlist name in `config.json`[qq_playlist_name]
4. run `python WYtoQQ.py`


* If you choose QQ to WY:
1. add your wy email account and password in `config.json`[wy_account, wy_password], currently only support WY email account.
2. copy qq playlist url in `config.json`[qq_playlist_url]
3. input wy user playlist url in `config.json`[wy_user_playlist_url]
4. run `python QQtoWY.py`

> If you are not sure how to input the correct url config, please see the screenshot in dir `example`. Or you can email me.

### windows exe
1. do #Step 1 and #Step 2 
2. run `win32/run.exe`
3. according the notice, input the driver absolute path.

---------------
## debug
you can use chrome driver.
1. Uncomment line 59 and line 64
2. download chrome driver
3. set driver path in `settings.py`

---------------
## enhancement
1. sync music.qq to music.163.
