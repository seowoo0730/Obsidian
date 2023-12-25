## `for`

```Python
for (초깃값; 조건; 실행 후 작업) {
  //code
}
```

```JavaScript
for (let i = 0; i < 10; i++) {
  console.log(i);
} //0123456789
```

---

## `while`

**소괄호 안의 조건이 참**이면 **중괄호 안의 코드를 실행**한다

```JavaScript
let i = 0;

while (i < 10) {
  console.log(i);
  i++;
} //0123456789
```

---

## `do while`

**먼저 한 번 실행** 하고 **소괄호 안의 조건이 참**이면 **중괄호 안의 코드를 실행**한다

```JavaScript
let i = 0;
do {
  console.log(i);
  i++;
} while (i < 0); //0
```