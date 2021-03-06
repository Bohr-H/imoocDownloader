# imoocDownloader
[![Build Status](https://travis-ci.org/webbought/imoocDownloader.svg?branch=v1.1.0)](https://travis-ci.org/webbought/imoocDownloader) 

`由于慕课网现在的视频播放机制已经跟写项目时有所改变，所以部分视频会无法下载，该项目也不再维护`

### 简介

imoocDownloader 用来爬取慕课网课程视频


### 安装

```shell
git clone https://github.com/webbought/imoocDownloader.git

cd imoocDownloader 

npm install
```



### Usage
```javascript
'use strict'

module.exports = {
    videoDir : './video',
    targets : [552,556,21,441,11]
}
```

##### 配置好config文件，执行 `node index.js`即可。 
 
### 指令模式
```shell
node index.js <command> <arguments>

Options:

-h, --help          output usage information
-V, --version       output the version number
-s, --search <n>    Search course specified by keywords
-l, --list <n>      Show the Chapters and Lessons by course Id
-d, --download <n>  Download the Course By course Id
```
    
#### example
```shell
node index.js --search mongodb
```
![search][1]

```shell
node index.js --list 578
```
![list][2]

```shell
node index.js --download 578
```

or

```shell
node index.js --download 75,578
```

![download][3]
```
课程目录
```
![course][4]
```
章节目录
```
![chapter][5]
```
视频目录
```
![video][6]


[1]: https://github.com/webbought/imoocDownloader/blob/master/img/1.png "search"
[2]: https://github.com/webbought/imoocDownloader/blob/master/img/2.png "list"
[3]: https://github.com/webbought/imoocDownloader/blob/master/img/3.png "download"
[4]: https://github.com/webbought/imoocDownloader/blob/master/img/4.png "course"
[5]: https://github.com/webbought/imoocDownloader/blob/master/img/5.png "chapter"
[6]: https://github.com/webbought/imoocDownloader/blob/master/img/6.png "video"
