**Python함수**



1. list 함수

```python
testList = [1,2,3,4]

// 리스트 내 원소 삽입
testList.append(5)
//내림차순 정렬
testList.sort(reverse = True)
//오름차순 정렬
testList.sort()

//특정 위치에 데이터 추가
testList.insert(2,3)

//특정값 count
testList.count(1)

//특정 값 삭제
testList.remove(1) //시간복잡도 때문에 remove 사용은 지양
```



2. 문자열

```python
data = "python World"

dataFront = "python"
dataRear = "World"

dataFront + " " + dataRear  # python World

dataFront * 2 #pythonpython

dataFront[1:3] #yt

```



3. 사전 자료형

```python
dictCase = dict()
dictCase['사과'] = 'apple'
dictCase['바나나'] = 'banana'
dictCase['코코넛'] = 'Coconut'
 
 # {'사과' : 'apple', '바나나' : 'banana', '코코넛':'Coconut'}

if '사과' in dictCase :
	print("사과는 존재한다")
    
    
# 키 데이터만 담은 리스트
key_list = data.keys()
value_list = data.values()

for key in key_list:
        print(data[key]) # Apple Banana Coconut
```



4. 집합자료형(Set)

- 중복 허용 X

- 순서 없음

- 데이터 존재 여부 체크시 유용

  ```python
  # 집합 자료형 초기화 방법 
  data = set([1,1,2,3,4,4,5])
  
  data = {1,2,3,4,5}
  
  # 집합 자료형 초기화 방법 
  a = set([1,2,3,4,5])
  b = {3,4,5,6,7}
  
  a | b # 합집합 {1,2,3,4,5,6,7}
  a & b # 교집합 {3,4,5}
  a - b # 차집합 {1,2}
  
  data = set([1,2,3])
  print(data)
  
  # 새로운 원소 추가
  data.add(4)
  
  # 새로운 원소 여러 개 추가
  data.update([5,6])
  
  # 특정한 값을 갖는 원소 삭제
  data.remove(3)
  
  print(data)
  ```

  