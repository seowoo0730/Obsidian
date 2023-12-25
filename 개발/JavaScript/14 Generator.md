**Generator**는 함수를 잠시 멈추었다 다시 실행하게 해준다

```JavaScript
function* fn() {
  try {
    console.log(1);
    yield 1;
    console.log(2);
    yield 2;
    console.log(3);
    console.log(4);
    yield 3;
    return `finish`;
  } catch (e) {
    console.log(e);
  }
}

const a = fn();
```

![[Untitled 7 3.png|Untitled 7 3.png]]

![[Untitled 1 4 1.png|Untitled 1 4 1.png]]

![[Untitled 2 4 1.png|Untitled 2 4 1.png]]