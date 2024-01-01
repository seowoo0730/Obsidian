## 화살표 함수 선언

![[/Untitled 3.png|Untitled 3.png]]

![[/Untitled 1 2.png|Untitled 1 2.png]]

```JavaScript
const sum = (number1, number2) => {
  return number1 + number2;
};

const sumResult = sum(1, 3);
console.log(sumResult);
```

```JavaScript
const sum = (number1, number2) => number1 + number2;

const sumResult = sum(1, 3);
console.log(sumResult);
```

**객체**를 반환할 때는 **소괄호**로 함수를 닫는다

![[/Untitled 2 3.png|Untitled 2 3.png]]