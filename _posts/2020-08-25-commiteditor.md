---
title: "Git commit editor"
author: Young Dean
date: 2020-08-25
categories: [Git]
tags: [Blog, Git]
toc: true
toc_sticky: true
---
# Git 커밋 편집기 변경하기

WSL을 이용해서 git을 사용하는 것에 맛이 들른 와중에

vi 설정까지 거의 마쳐 기분이 좋았는데 

git commit 명령어만 사용하면 다른 편집기가 나와서 매우 불편했었다. 

그래서 이를 바꿀 수 있는 명령어를 찾았다. 

```
$git config --global core.editor vim
```

이 때 vim이 아닌 다른 편집기를 이용하고 싶다면 다른 편집기를 입력하면 된다.

변경된 사항은 .gitconfig의 내용을 확인하면 알 수 있다. 

그리고 commit을 원하던 vi 편집기를 이용할 수 있었다. 
