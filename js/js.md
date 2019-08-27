# javascript

## let, const
- var : function-scoped, 재선언 가능
- let : block-scoped, 재선언 불가능, 재할당 가능
-  const : block-scoped, 재선언 불가능, 재할당 불가능



### apply, call

- fun.apply([thisObj[,argArray])
- fun.call([thisObj[, arg[, arg2[, ...]]]])
- 그냥 호출하는 것이 아니라 this를 함수의 인자로 넘김으로써, this의 값을 사용할 수도, 변경 할 수도 있게 된다