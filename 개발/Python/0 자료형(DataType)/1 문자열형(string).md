## 문자열형(string)

```Python
print('hello')
```

### 슬라이싱(slicing)

문자열에서 **특정한 문자** 만을 가지고 올 수 있다

**a[이상:미만:간격]**

```Python
a = '1234567890'
print(a[1])  # 2
print(a[-1])  # 0
print(a[:-1])  # 123456789
print(a[::2])  # 13579
print(a[::-1])  # 0987654321
```

### 문자열 포맷

```Python
print('나는 %d살입니다.' % 20)  # 나는 20살입니다.
print('나는 %s를 배웁니다.' % 'Python')  # 나는 Python를 배웁니다.
print('Python은 %c로 시작합니다.' % 'P')  # Python은 P로 시작합니다.
print('%0.2f' % 2.1234)  # 2.12
```

```Python
print('나는 {}살 {}입니다.'.format(14, '이서우'))  # 나는 14살 이서우입니다.
```

```Python
print('나는 {1}살 {0}입니다.'.format('이서우', 14))  # 나는 14살 이서우입니다.
```

```Python
age = 14
name = '이서우'
print(f'나는 {age}살 {name}입니다.')  # 나는 14살 이서우입니다.
```

### 이스케이프 문자

### `\`

문자 앞에 `\`(이스케이프 문자)를 붙이면 **따옴표가 아닌 문자**로 인식한다

### `\n`

문자 앞에 `\n`(이스케이프 문자)를 붙이면 **줄바꿈**을 한다

```Python
print("I'm fine thank you! \\n\\"and you?\\"")
# I'm fine thank you!
# "and you?"
```

### `\\`

문자 `\\`를 붙이면 **\**이다

```Python
print('C:\\Users\\이서우')  # C:\\Users\\이서우
```

### `\r`

문자 `\r`를 붙이면 문자를 **앞으로 이동**한다

```Python
print('Red Apple \rPine')  # PineApple
```

### `\b`

문자 `\b`를 붙이면 문자를 **앞 한 글자를 삭제**한다

```Python
print('Redd\b Apple')  # Red Apple
```

### `\t`

문자 `\t`를 붙이면 문자를 **tab**을 누른 것과 같다

```Python
print('Redd\b \tApple')  # Red     Apple
```