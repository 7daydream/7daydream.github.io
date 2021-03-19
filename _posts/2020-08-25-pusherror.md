---
title: "git push 오류 failed to push some refs to "
author: Young Dean
date: 2020-08-25
categories: [Git]
tags: [Blog, git]
toc: true
toc_sticky: true
---
# git push 오류 failed to push some refs to 

노트북을 새로 사고 세팅을 한 후 github에 push를 하던 중 다음과 같은 오류가 발생했다.

```
error: failed to push some refs to 'http://github.com/~'
```

다행이 아래에 hint라는 내용도 같이 있었다.

```
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
```

local과 remote의 repository의 내용이 다르기 때문에 발생한 일이었다. 

따라서 remote의 변경사항(local과 애초에 다른 부분)을 integrate 하는 과정이 필요하다는 것이다.

github에서 먼저 repository를 만들고 노트북에 같은 폴더를 만든 후 
git push를 하려던 것이 화근이었다. 

그래서 다시 git pull 명령어를 통해 local과 remote와 같은 내용으로 맞춘 후
다시 git push 명령어를 입력하니 문제없이 push가 진행되었다. 

끝
