객체는 **`키:값`** **`key:value`****로 이루어진 데이터를 여러 개 할당**할 수 있다

```run-python
student1 = {'korean_score': 95,
            'math_score': 100,
            'english_score': 90}

print(student1)  # {'korean_score': 95, 'math_score': 100, 'english_score': 90}
```

```run-python
print(student1('science_score'))
print(student1('math_score'))  # TypeError: 'dict' object is not callable
```

```run-python
print(student1.get('science_score'))  # None
print(student1.get('math_score'))  # 100
```

### 데이터 추가

```run-python
student1['science_score'] = 100
student1['english_score'] = 95
print(student1)
# {'korean_score': 95, 'math_score': 100, 'english_score': 95, 'science_score': 100}
```

## 데이터 삭제

```run-python
del student1['english_score']
print(student1)  # {'korean_score': 95, 'math_score': 100}
```

---

### key 출력

```run-python
print(student1.keys())
# dict_keys(['korean_score', 'math_score', 'english_score'])
```

### value 출력

```run-python
print(student1.values())  # dict_values([95, 100, 90])
```

### key, value 출력

```run-python
print(student1.items())
\#dict_items([('korean_score', 95), ('math_score', 100), ('english_score', 90)])
```

### `get`

```run-python

student1 = {'korean_score': 95,
            'math_score': 100,
            'english_score': 90}

print(student1.get(12345))  # None
```

### `in`

```run-python
student1 = {'korean_score': 95,
            'math_score': 100,
            'english_score': 90}

print('science_score' in student1)  # False
```

---

### `clear`

```run-python
student1.clear()
print(student1)  # {}
```