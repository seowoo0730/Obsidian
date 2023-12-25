## `async`

함수 앞에 `async`를 붙이면 **비동기 적**이게 된다

```JavaScript
async function promise() {
  return `seowoo`;
}

async function print() {
  const name = await promise();
  return name;
}

print().then(console.log); //seowoo
```

**try, catch**로 **오류 처리**를 할 수 있다