`key`와 `value`가 **일치하면 그 안의 코드를 실행**한다

```JavaScript
switch (key) {
  case (value):
    //code
    break;
  case (value):
    //code
    break;
  case (value):
    //code
    break;
  default:
    //code
    break;
}
```

```JavaScript
let animal = `dog`;

switch (animal) {
  case `cat`:
    console.log(`야옹`);
    break;
  case `dog`:
    console.log(`멍멍`);
    break;
  case `cow`:
    console.log(`음메`);
    break;
  default:
    console.log(`동물 소리가 없습니다.`);
    break;
} //멍멍
```