## `if`

**소괄호 안의 조건이 참**이면 **중괄호 안의 코드를 실행**한다

```run-javascript
if (10 < 20) {
  console.log(`10은 20보다 작다.`);
} //10은 20보다 작다.
```

---

## `else`

**소괄호 안의 조건이 거짓**이면 **중괄호 안의 코드를 실행**한다

```run-javascript
if (30 < 20) {
  console.log(`30은 20보다 작다.`);
} else {
  console.log(`30은 20보다 작지 않다.`);
} //30은 20보다 작지 않다.
```

---

## `else if`

**앞 조건문이 거**짓이면 **뒤 조건문이 순차적으로 실행**된다

```run-javascript
if (30 < 20) {
  console.log(`30은 20보다 크다.`);
} else if (30 < 25) {
  console.log(`30은 25보다 크다.`);
} else if (30 < 30) {
  console.log(`30은 30보다 크다.`);
} else if (30 < 35) {
  console.log(`30은 35보다 크다.`);
} //30은 35보다 크다.
```