---
title: "Git push 시 password authentication 오류 발생"
author: Young Dean
date: 2021-09-19
categories: [error]
tags: [error, git]
toc: true
toc_sticky: true
---

# Git password authentication 관련

요즘 블로그에 신경을 못 썼는데 다시 마음을 다잡고 글을 써보기로 했다. 

간만에 블로그에 수정할 것이 생겨 `git push`를 하였으나 다음과 같은 오류가 발생했다. 

```
remote: Support for password authentication was removed on August 13, 2021.
Please use a personal access token instead.                                  
remote: Please see https://github.blog/2020-12-15-token-authentication-requirements-for-git-operations/ for more information.
fatal: Authentication failed for ~~
```

예전부터 메일로 패스워드 인증이 끝난다는 이야기를 얼핏 봤었지만 따로 조치를 취하지 않았었다...

찾아보니 password를 이용한 인증 대신 토큰 기반의 인증을 하겠다는 것이다. 

간단하게 방법을 정리하면 다음과 같다. 

> 1. `Github`로그인 후 `setting` 메뉴 이동
> 2. `Developer` 메뉴 이동
> 3. `Personal access tokens` 메뉴 이동
> 4. `Generate new token` 버튼 클릭
> 5. 자신이 허용하는 알맞은 세팅 완료 후 토큰 발생 시 토큰을 복사

이 때 주의할 점은 토큰은 한 번 밖에 보여주지 않기 때문에 꼭 **복사**를 해주고 안전한 곳에 저장을 해두어야 한다.

그리고 앞으로는 패스워드 칸에 이 토큰을 붙여넣어주어 인증을 완료하면 된다.

~~근데 많이 불편한듯...~~
