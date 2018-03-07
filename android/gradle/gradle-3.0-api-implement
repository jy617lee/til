## gradle 3.0 api, implement 정리


compile 키워드가 deprecate되었고 implement, api 키워드가 추가되었다. dependent한 라이브러리에 직접 접근이 가능한지에 따라 두 키워드가 나누어진다. 

### api 키워드
deprecate된 compile 키워드와 동일하다. libraryA가 libraryB에 dependent할 경우 app에서는 A, B에 모두 직접 접근이 가능하며 B가 변경될 경우 A, B, 앱 모듈을 모두 recompile 해야 한다. 

#####  gradle project
```gradle
dependencies {
	api project(path: ':libraryB')
}
```
#####  gradle app
```gradle
dependencies {
	api project(path: ':libraryA')
}
```

#####  app
```java
public void foo(){
	A a = new A();
    B b = new B();
}
```
### implement 키워드
libraryA가 libraryB에 dependent할 경우 app에서는 A에만 직접 접근이 가능하며, B가 변경될 경우 A, B만 recompile하면 된다.

##### gradle project
```gradle
dependencies {
	. . . .
	implementation project(path: ':libraryA')		
}
```
#####  gradle app
```gradle
dependencies {
	. . . .
	implementation project(path: ':libraryA')		
}
```

#####  app
```java
public void foo(){
	A a = new A();
    B b = new B(); <-- error
}
```


###참고한 링크 
1. 한글 번역: https://sikeeoh.github.io/2017/08/28/implementation-vs-api-android-gradle-plugin-3/
2. 영문 : https://medium.com/mindorks/implementation-vs-api-in-gradle-3-0-494c817a6fa