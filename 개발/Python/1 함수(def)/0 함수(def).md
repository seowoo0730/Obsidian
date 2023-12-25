**하나의 작업을 처리하기 위해 연관된 코드들을 모아** 놓는 자료형

## 함수 선언

```Python
def function_name(args):
  \#code
```

### 함수 호출하기

```Python
def function_name():
    print('Function')


function_name()  # Function
```

---

## 인수, 매개변수(parameter)

```Python
def add(a, b):
    print(a/b)

add(b=2, a=4)  # 2.0
```

### 기본값

```Python
def introduce(name, age=14):
    print('이름: {0} 나이: {1}'.format(name, age))


introduce('이서우')  # 이름: 이서우 나이: 14
```

### 가변인자

```Python
def introduce(name, *lang):
    print('이름: {0}'.format(name), end=" ")
    for lang in lang:
        print(lang, end=" ")


introduce('이서우', 'python', 'java', 'javascript')
# 이름: 이서우 python java javascript
```

---

## 지역변수

지역변수는 **함수 내에서만 사용**할 수 있는 변수이다

## 전역변수

전역변수는 **함수 외에 있는 변수**이다

### 전역변수 사용법

```Python
name = '이서우'

def introduce():
    global name
    print('이름: {0}'.format(name))

introduce()  # 이름: 이서우
```

프로그램이 복잡해질 수 있어 `return`을 더 많이 사용하자

### lambda

**함수를 한 줄**로 간결하게 만들 때 사용한다

```Python
list = [lambda a, b:a+b, lambda a, b:a*b]
print(list[1](2, 4))  # 8
```

---

## return

```JavaScript
def add1(a, b):
    return a+b


def add2(c, d):
    return c+d


def add3(e, f):
    return e+f

result1 = add1(2, 3)
result2 = add2(3, 4)
result3 = add3(result1, result2)
print(result1, result2, result3)  # 5 7 12
```

![[Untitled 14.png|Untitled 14.png]]

[[개발/Python/1 함수(def)/1 화살표 함수(arrow function)|1 화살표 함수(arrow function)]]

[[2 랜덤 함수]]

[[3 문자열 처리 함수]]