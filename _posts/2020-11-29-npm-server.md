---
layout: post
title: npm 서버 실행 오류(npm ERR! code ELIFECYCLE)
tags: [npm, 오류 해결, server]
color: brown
author: aerimforest
excerpt_separator: <!--more-->
---

서버를 연결하고 `npm start` 명령어를 입력했을 때, 아래와 같은 에러 메세지가 뜨는 경우가 있다.
> npm ERR! code ELIFECYCLE
&nbsp;&nbsp;


### 해결 방법


```bash
$ pm cache clean --force
$ rm -rf node_modules // node_modules 폴더 제거
$ npm install
$ npm start
```




이후 `http://localhost:포트넘버`로 접속하면 잘 작동하는 것을 볼 수 있다! 


[^1]: 
    {% include citation.html key="ref1" %}
