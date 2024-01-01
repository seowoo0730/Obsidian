배열에는 **하나의 변수에 여러 개의 데이터를 할당**할 수 있다

```Python
list = [10, 'abc', 5 > 7]
print(list)  # [10, 'abc', False]
```

## `index`

인덱스(index)를 사용하면 배열에서 특정한 값의 위치를 가지고 올 수 있다

```Python
list = [10, 'abc', 5 > 7]
print(list.index('abc'))  # 1
```

### 슬라이싱(slicing)

문자열에서 **특정한 값** 만을 가지고 올 수 있다

**a[이상:미만:간격]**

```Python
a = '1234567890'
a = [1, 2, 3, 4, 5, 6, 7, 8, 9, 0]
print(a[1])  # 2
print(a[-1])  # 0
print(a[:-1])  # [1, 2, 3, 4, 5, 6, 7, 8, 9]
print(a[::2])  # [1, 3, 5, 7, 9]
print(a[::-1])  # [0, 9, 8, 7, 6, 5, 4, 3, 2, 1]
```

### `len` 리스트의 길이

```Python
a = [1, 2, 3, 4, 5, 6, 7, 8, 9, 0]
print(len(a)) # 10
```

### `sum` 합

```Python
a = [1, 2, 3, 4, 5, 6, 7, 8, 9, 0]
print(sum(a)) # 45
```

### `min`, `max`

```Python
a = [1, 2, 3, 4, 5, 6, 7, 8, 9, 0]
print(min(a)) # 0
print(max(a)) # 9
```

### `append` 데이터 추가

```Python
list = [10, 'abc', 5 > 7]
list.append(2*5)
print(list)  # [10, 'abc', False, 10]
```

### `insert` 데이터 사이에 추가

```Python
list = [10, 'abc', 5 > 7]
list.insert(1, 2*5)
print(list)  # [10, 10, 'abc', False]
```

### `pop` 가장 뒤의 데이터 삭제

```Python
list = [10, 'abc', 5 > 7]
list.pop()
print(list)  # [10, 'abc']
```

### `count` 개수 세기

```Python
list = [10, 5+5, 'abc', 5 > 7]
print(str(list.count(10)) + '개')  # 2개
```

### `sort` 정렬

```Python
list = [10, 5+5, 2, 7 - 10]
list.sort()
print(list)  # [-3, 2, 10, 10]
```

### `reverse` 순서 뒤집기

```Python
list = [10, 5+5, 2, 7 - 10]
list.sort()
print(list)  # [-3, 2, 10, 10]
list.reverse()
print(list)  # [10, 10, 2, -3]
```

### `clear` 모두 삭제

```Python
list = [10, 5+5, 2, 7 - 10]
list.clear()
print(list)  # []
```

### `remove` 삭제

```Python
list = [10, 5+5, 2, 7 - 10]
list.remove(10)
print(list) # [10, 2, -3]
```

### `extend`

```Python
list1 = [10, 5+5, 2, 7 - 10]
list2= [98,99]
list1.extend(list2)
print(list1) # [10, 10, 2, -3, 98, 99]
```