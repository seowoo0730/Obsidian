## 화살표 함수 선언

![[Untitled 9 1.png|Untitled 9 1.png]]

![[Untitled 1 5 1.png|Untitled 1 5 1.png]]

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
console.log(sumResult); //4
```

**객체**를 반환할 때는 **소괄호**로 함수를 닫는다