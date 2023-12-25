## 원시 타입(primitive type)

### **숫자형(number)**

```JavaScript
console.log(typeof 1); //number
```

### 논리형(boolean)

참은 true 거짓은 false로 나타낸다

```JavaScript
let bool = true;
console.log(bool); //ture
```

```JavaScript
let bool2 = 5 > 7;
console.log(bool2); //false
```

### null

null은 **명시적으로 변수 공간이 비었음**을 나타낸다

```JavaScript
let num = null;
console.log(num); //null
```

### undefined

**변수에 아무런 값도 할당하지 않으면** undefined 자료형을 가지게 된다

```JavaScript
let num;
console.log(num); //undefind
```

### Symbol

Symbol은 **값이 같아도 다르다고 해 유일**성을 보장한다

```JavaScript
let a = Symbol('id');
let b = Symbol('id');
console.log(a === b);
//false
```

## 참조 타입(reference type)

### 배열(array)

```JavaScript
console.log(typeof []); //arry
```

### 객체(object)

```JavaScript
console.log(typeof {}); //object
```

### 함수(function)

```JavaScript
console.log(typeof function(){}); //funtion
```

[[개발/JavaScript/자료형(DataType)/1 문자열형(string)]]