## generator와 yield

- generator : 딱 한번만 사용 가능한 iterator. 모든 값을 메모리에 올려두는 것이 아니라 한번 실행한 후에 날려버린다
- yield : generator를 return하는 keyword

```python
def createGenerator():
	mylist = range(3)
	for i in mylist:
		yield i*i

# createGenerator 함수가 도는 것이 아니라
# yield 뒤의 generator 객체만 가져온다
# 원래는 한 번 generator를 생성하는 코드를 실행하고 나면 빈 것으로 여겨지지만 yield가 있으면 재활용 가능하다. 
mygenerator = createGenerator() # create a generator
print(mygenerator) 
>> 0
>> 1
>> 4
```

- 참고 : https://stackoverflow.com/questions/231767/what-does-the-yield-keyword-do