---
layout: post
title: npm 서버 실행 오류(npm ERR! code ELIFECYCLE)
tags: [npm, 오류 해결, Server]
color: brown
author: aerimforest
excerpt_separator: <!--more-->
---

<br><br>

<span style="font-size:1;">서버를 연결하고 `npm start` 명령어를 입력했을 때, 아래와 같은 에러 메세지가 뜨는 경우가 있다.</span>

> ##### npm ERR! code ELIFECYCLE

<br><br>
### 해결 방법


```bash
$ npm cache clean --force
$ rm -rf node_modules // node_modules 폴더 제거
$ npm install
$ npm start
```



<br><br>

##### 이후 `http://localhost:포트넘버`로 접속하면 잘 작동하는 것을 볼 수 있다! 

<br><br>
### 서버 종료
> ##### ctrl + C
