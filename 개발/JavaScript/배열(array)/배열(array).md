![[/Untitled 2.png|Untitled 2.png]]

배열에는 **하나의 변수에 여러 개의 데이터를 할당**할 수 있다

```JavaScript
let arr = [10, `abc`, 5 > 7, null];
console.log(arr); //[10, `abc`, 5 > 7, null];
```

## 인덱스(index)

인덱스(index)를 사용하면 배열에서 특정한 값 만을 가지고 올 수 있다

```JavaScript
console.log(arr[0]); //10
```

## 개수

```JavaScript

console.log(arr.length); //4
```

## 추가

```JavaScript
arr[4] = `hello`;
console.log(arr); //[10, 'abc', false, null, 'hello']
```

  

### `splice`

```JavaScript
let arr = [10, `abc`, 5 > 7, null];
arr.splice(2, 2);
console.log(arr); //[10, 'abc']
```

![[/Untitled 1 2.png|Untitled 1 2.png]]

```JavaScript
arr.splice(2, 2, `de`);
console.log(arr); //[10, 'abc', 'de']
```

![[/Untitled 2 2.png|Untitled 2 2.png]]

### `slice` 자르고 새 배열 만들기

```JavaScript
let arr = [10, `abc`, 5 > 7, null];
console.log(arr.slice(0, 2)); //[10, 'abc']
```

### `push`

```JavaScript
arr.push(`hello`);
console.log(arr); //[10, 'abc', false, null, 'hello']
```

### `concat`

```JavaScript
let arr = [10, `abc`, 5 > 7, null];
arr = arr.concat([`hello`, 11]);
console.log(arr); //[10, 'abc', false, null, 'hello', 11]
```

### `unshift`

```JavaScript
let arr = [10, `abc`, 5 > 7, null];
arr.unshift(`hello`, 9);
console.log(arr); //['hello', 9, 10, 'abc', false, null]
```

## 제거

### `shift`

```JavaScript
arr.shift();
console.log(arr); //['abc', false, null]
```

### `pop`

```JavaScript
arr.pop();
console.log(arr); //[10, 'abc', false]
```

## 정렬

### `sort`

```JavaScript
let arr = [10, 9, 999, -1];
arr.sort();
console.log(arr); //[-1, 10, 9, 999]
```

### `reverse`

```JavaScript
let arr = [`a`, `g`, `c`, `b`, `x`];
arr.reverse();
console.log(arr); //['x', 'b', 'c', 'g', 'a']
```

### `indexOf` 위치 찾기

```JavaScript
let arr = [`a`, `b`, `c`, `d`, `e`];
console.log(arr.indexOf(`c`)); //2
```

### `lastIndexOf` 위치 찾기2

```JavaScript
let arr = [`a`, `b`, `c`, `d`, `e`, `c`];
console.log(arr.lastIndexOf(`c`)); //5
```

### `includes` 포함

```JavaScript
let a = `Hi I'm Lee`;
console.log(a.includes(`Hello`)); //false
```

### `find`, `findIndex`

함수를 사용해 만족하는 값을 **하나** 반환한다

### `filter`

![[/Untitled 3.png|Untitled 3.png]]

함수를 사용해 만족하는 값을 **모두** 반환한다

![[/Untitled 4.png|Untitled 4.png]]

### `reduce`

```JavaScript
arr.reduce((누적 계산값, 현재 배열 요소, 배열 위치, 배열) => {
  //code
}, 초깃값);
```

```JavaScript
let arr = [1, 2, 3, 4, 5];

const result = arr.reduce((prev, cur) => {
  return prev + cur;
}, 0);

console.log(result); //15
```

### `forEach`

```JavaScript
arr = [`one`, `two`, `three`];
arr.forEach(function (item, index, array) {
  console.log(item, index, array);
});
//one 0 ['one', 'two', 'three']
//two 1 ['one', 'two', 'three']
//three 2 ['one', 'two', 'three']
```

```JavaScript
arr = [`one`, `two`, `three`];
arr.forEach((item) => console.log(item));
//one
//two
//three
```

### `join` 문자열 만들기

```JavaScript
let arr = [`korea`, `japan`];
str = arr.join(` vs `);
console.log(str); //korea vs japan
```

### `map` 특정값 변경

```JavaScript
arr = [1, 2, 3, 4];
let result = arr.map((item) => item * 2);
console.log(result); //[2, 4, 6, 8]
```

### `some` 판별 함수 통과 테스트(or)

```JavaScript
arr = [1, 2, 3, 4];
let even = arr.some((item) => item % 2 === 0);
console.log(even); //true
```

### `every` 판별 함수 통과(and)

```JavaScript
arr = [1, 2, 3, 4];
let even = arr.every((item) => item % 2 === 0);
console.log(even); //false
```