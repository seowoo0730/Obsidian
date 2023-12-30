## call

**모든 함수**에서 사용 가능 `this`를 **특정 값으로 지정** 가능

```JavaScript
const tom = { name: `Tom` };
function showName() {
  console.log(this.name);
}
showName.call(tom); //Tom
```

## apply

매개변수를 **배열**로 받음

## bind

를 **영구히** 바꿈