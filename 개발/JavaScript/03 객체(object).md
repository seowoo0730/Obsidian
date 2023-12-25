객체는 **`key:value`****로 이루어진 데이터를 여러 개 할당**할 수 있다

```JavaScript
let student1 = {
  koreanScore: 95,
  mathScore: 100,
  englishScore: 90,
};

console.log(student1); // {koreanScore: 95, mathScore: 100, englishScore: 90}
```

```JavaScript
let student1 = {
  koreanScore: 95,
  mathScore: 100,
  englishScore: 90,
};

console.log(student1[`mathScore`]); //100
```

```JavaScript
let student1 = {
  koreanScore: 95,
  mathScore: 100,
  englishScore: 90,
};

console.log(student1.englishScore); //90
```

## 추가

```JavaScript
let student1 = {
  koreanScore: 95,
  mathScore: 100,
  englishScore: 90,
};

student1.scienceScore = 100;
console.log(student1);
// {koreanScore: 95, mathScore: 100, englishScore: 90, scienceScore: 100}
```

## 삭제

```JavaScript
let student1 = {
  koreanScore: 95,
  mathScore: 100,
  englishScore: 90,
};

delete student1.mathScore;
console.log(student1); // {koreanScore: 95, englishScore: 90}
```

## 확인

```JavaScript
let student1 = {
  koreanScore: 95,
  mathScore: 100,
  englishScore: 90,
};

console.log('scienceScore' in student1); // false
```