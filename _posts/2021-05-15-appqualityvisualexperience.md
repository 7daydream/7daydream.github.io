---
title: "App Quality Visual Experience"
author: Young Dean
date: 2021-05-15
categories: [Android]
tags: [Android]
toc: true
toc_sticky: true
---

> [App Quality : Visual Experience](https://youtu.be/uUWqUp_HeNs)
> Android Developer 유튜브 채널의 동영상을 번역하였습니다. 
> 오역 및 의역이 있을 수 있을 수 있습니다...

Android 앱의 visual experience는 사용자가 앱 품질에 대해서 평가시 중요한 부분을 차지한다. 

최신 Android 디자인 지침으로 최신 상태를 유지한다면 앱에 소속감이 생기고 사용성을 개선할 수 있다. 

다음은 visual experience를 위한 새로운 핵심 앱 품질 체크리스트에 대해 4가지 권장 사항이다. 

### 먼저, Material 디자인을 사용하는 것이 좋다.

Material 디자인이란 platform default components가 아닌 앱을 빌드하기 위한 components이다. 

안드로이드의 전반적인 외형과 느낌은 오늘날과 같은 Material 디자인 시스템으로 크게 변경되었다. 

앱에 현대적인 모양과 느낌을 제공하는 것 외에도 material 디자인 컴포넌트는 많은 시간을 절약할 수 있는 복잡한 위젯을 제공한다. 

예를 들어 time picker가 있는데, 이걸 처음부터 코딩한다고 생각하는 것보다는 material 디자인 컴포넌트를 한번만 import하면 된다. 

자세한 내용은 material 디자인 컴포넌트에 대한 최신 안드로이드 개발 시리즈를 확인하면 된다. 

### 두 번째는 어두운 테마이다.

이 기능은 Android 10 도입 이래로 사용자들의 관심을 끌었다. 

현재 activate 안드로이드 장치의 1/3에서 OS수준으로 지원된다. 

앱에서 material 디자인 컴포넌트를 사용하는 경우 어두운 테마를 쉽게 채택할 수 있다. 

자세한 내용은 dark theme 개발 가이드를 확인하면 된다. 

### 다음은 gesture navigation이다. 

안드로이드를 사용하는 경우 사용자는 화면 양쪽에서 안쪽으로 스와이프하여 뒤로 탐색하거나 하단의 버튼 탐색 표시 줄을 없앨 수 있다. 

이 경우 사용자에게 더 많은 화면 공간을 제공할 수 있다. 

안드로이드에서 edge-to-edge 스크린이 대중화되면서 entry 레벨 장치에서도 앱이 gesture navigation을 신경쓰며 개발하는 것이 중요해졌다. 

예를 들면 SeekBar를 사용하는 경우 스와이프했다고 평소처럼 gesture navigation이 되면 안된다. 

또한 사용자 지정 컴포넌트를 만드는 경우도 gesture navigation을 고려해야 한다. 

### 마지막으로, 앱의 정확한 State를 유지해야 한다. 

사용자가 양식을 작성하는데 필요한 정보를 얻기 위해 실수로 앱을 종료하거나 앱을 전환하는 경우를 상상하자.

재개시, 사용자가 몇 분 이내로 빠르게 다시 화면을 전환한다면 이전과 동일한 상태로 재개되어야 한다. 

사용자가 나중에 다시 시작하는 경우 앱 개발자는 앱의 context에 따라서 사용자를 기본 홈 화면으로 이동하거나 마지막 상태로 다시 시작할 수 있다. 

---
앱의 퀄리티를 높일 수 있는 네 가지 방안을 알아볼 수 있었다. 

특히 Material Design 사용법과 마지막의 앱의 생명주기를 더 자세히 알아보고 꼼꼼히 코딩할 수 있는 개발자가 되고 싶다는 생각을 했다. 
