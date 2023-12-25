```JavaScript
console.log(`I'm iron man`)
```

`` ` ``를 사용하면 **안에 다른 따옴표가 있어도 상관없이 문자열로 인식**한다

그리고 이를 이용하면 **문자열에 변수를 대입해 사용**할 수 있다

```JavaScript
let name = `이서우`;
console.log(`Hello my name is ${name}`);
// Hello my name is 이서우
```

![[Untitled 6 3.png|Untitled 6 3.png]]

```JavaScript
console.log(`Hello I'm ${13 + 1}years old`);
// Hello I'm 14years old
```