---
title: View Binding 뷰 바인딩
author: Young Dean
date: 2021-06-20
categories: [Android]
tags: [Android]
toc: true
toc_sticky: true
---

# View binding
이전에 사용하던 ```kotlin extention```은 deprecate되고 ```findViewById```를 사용하는 것 보다는 ```View Binding```을 사용하는 것이 차후 코드를 간결하게 하고 안드로이드에 대한 이해를 높일 수 있을 것이라 생각해서 기본적인 사용법을 정리하고자 한다. 

## 사용
우선 ```gradle``` 설정은 다음과 같다. 
이 때 안드로이드 스튜디오 버전마다 조금은 다르다고 하는데 4.2.1버전에서 진행하였다.

```
android {
... // 기본적으로 작성된 내용들 생략
	viewBinding {
		enabled = true
	}
}
```

그 후 activity_main.xml 파일을 기준으로 설명을하면 ```ActivityMainBinding```의 형태로 클래스 이름을 활용한다. 

```kotlin
class MainActivity : AppCompatActivity() {
	
	private lateinit var binding : ActivityMainBinding

	override fun onCreate(savedInstanceState: Bundle?) {
		super.onCreate(savedInstanceState)
		binding = ActivityMainBinding.inflate(layoutInflater)
		val view = binding.root
		setContentView(view)
	}
	
}
```

이후 activity_main.xml 파일에 button1이라는 id를 가진 ```ButtonView```가 있다면 ```binding.button1.setOnClickListener()```와 같이 ```kotlin extention```사용하듯이 사용하면 된다. 

```Fragment```나 ```RecyclerView```, ```Adapter```등에서 또 사용방법이 다르다고 하는데 더 공부해서 정리해야겠다. 
