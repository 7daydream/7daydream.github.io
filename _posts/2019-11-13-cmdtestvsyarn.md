---
title: "우분투 환경 cmdtest vs yarn"
author: Young Dean
date: 2019-11-13
categories: [Ubuntu, error]
tags: [Blog, 우분투]
pin: true
toc: true
toc_sticky: true
---

# 우분투 환경에서 cmdtest 대신 yarn 설치하기

클론 코딩 연습을 하던 중 yarn을 설치할 일이 생겨 
yarn을 설치하려 시도했었다. 

```
sudo apt install yarn
```

정말 간단하게 설치되나 했더니,
yarn 대신 cmdtest가 설치된다는 글이 떴다. 

그렇게 설치 후에 이상한 점을 눈치 챘을 때는
``` 
yarn init 
```

이 yarn 명령어로 프로젝트 기본 설정을 
진행하려 했을 때, 오류가 발생했다. 
오류의 내용은 아래와 같았다. 

```
[Errno 2] No such file or directory: 'init'
```

아마 yarn 뒤에 다른 명령어를 입력해도 비슷한 
error가 발생했을 것이다. 

cmdtest말고 yarn을 설치하기 위해서는
일단 cmdtest와 yarn을 다시 지워준다.

```
sudo apt remove cmdtest
sudo apt remove yarn
```

apt 명령어로 cmdtest와 yarn을 지운 후,
yarn 공식 repository를 추가해준다.
추가하는 명령어는 다음과 같다.

```
$curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add -

$echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list
```

위의 명령어를 실행한 후 yarn 을 다시 설치한다.

```
$sudo apt-get update && sudo apt-get install yarn

$yarn install
```

이후에는 yarn이 잘 실행되었다. cmdtest 잘 가라..
