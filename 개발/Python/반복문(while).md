## `while`

**소괄호 안의 조건이 참**이면 **중괄호 안의 코드를 반복해서 실행**한다

```Python
i = 0

while i < 10:
    print(i)
    i = i + 1
# 0 1 2 3 4 5 6 7 8 9
```

### `break`

```Python
python_file = open('python.txt', 'r', encoding='utf8')
while True:
    line = python_file.readline()
    if not line:
        break
    print(line)
python_file.close()
# Hello World

# hi

# hello
```