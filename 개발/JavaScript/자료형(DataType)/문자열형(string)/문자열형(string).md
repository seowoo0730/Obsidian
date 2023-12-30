```JavaScript
console.log(typeof `abc`); //string
```

## 이스케이프 문자

### `\`

문자 앞에 `\`(이스케이프 문자)를 붙이면 **따옴표가 아닌 문자**로 인식한다

```JavaScript
console.log("I'm fine thank you! \"and you?\"");
```

## `\n`

문자 앞에 `\n`(이스케이프 문자)를 붙이면 **줄바꿈**을 한다

```JavaScript
console.log("I'm fine thank you!\nand you?");
// I'm fine thank you!
// and you?
```

### `length` 문자의 길이

```JavaScript
console.log('coding everybody'.length); //16
```

### `toUpperCase`, `toLowerCase` 대소문자

```JavaScript
let a = `Hi I'm Lee`;
console.log(a.toUpperCase()); //HI I'M LEE
console.log(a.toLowerCase()); //hi i'm lee
```

### `indexOf` 위치 찾기

```JavaScript
	let a = `Hi I'm Lee`;
console.log(a.indexOf(`Lee`)); //7
```

### `slice`

```JavaScript
let a = `Hi I'm Lee`;
console.log(a.slice(7)); //Lee
console.log(a.slice(3, 6)); //I'm
console.log(a.slice(3, -4)); //I'm
```

### `substring`

```JavaScript
let a = `Hi I'm Lee`;
console.log(a.substring(10, 7)); //Lee
```

### `substr`

```JavaScript
let a = `Hi I'm Lee`;
console.log(a.substr(0, 2)); //Hi
```

![[/Untitled 8.png|Untitled 8.png]]

### `trim` 앞, 뒤 공백 제거

```JavaScript
let a = `  Hi I'm Lee   `;
console.log(a.trim()); //Hi I'm Lee
```

### `repeat` 반복

```JavaScript
let a = `Hi I'm Lee`;
console.log(a.repeat(3)); //Hi I'm LeeHi I'm LeeHi I'm Lee
```

### `includes` 포함

```JavaScript
let a = `Hi I'm Lee`;
console.log(a.includes(`Hello`)); //false
```

### `split` 문자열 나누기

```Python
a = `hello my name is seowoo`;
console.log(a.split(` `)); //['hello', 'my', 'name', 'is', 'seowoo']
```

## `replace`

```JavaScript
const a = `Hi I'm Lee`;
console.log(a.replace(`Lee`, `seowoo`)); //Hi I'm seowoo
```