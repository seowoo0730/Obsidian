## Producer

```run-javascript
const promise = new Promise((resolve, reject) => {
  setTimeout(() => {
    resolve(`seowoo`);
  }, 2000);
});
```

## Consumers

### `then`

```run-javascript
const promise = new Promise((resolve, reject) => {
  setTimeout(() => {
    resolve(`seowoo`);
  }, 2000);
});

promise.then((value) => {
  console.log(value); //seowoo
});
```

### `catch`

```run-javascript
const promise = new Promise((resolve, reject) => {
  setTimeout(() => {
    reject(new Error('no network'));
  }, 2000);
});

promise
  .then((value) => {
    console.log(value);
  })
  .catch((err) => {
    console.err(err); //Error: no network
  });
```

### `finally`

```run-javascript
const promise = new Promise((resolve, reject) => {
  setTimeout(() => {
    resolve(`seowoo`);
    reject(new Error('no network'));
  }, 2000);
});

promise
  .then((value) => {
    console.log(value);
  })
  .catch((err) => {
    console.err(err); //Error: no network
  })
  .finally(() => {
    console.log(`finally`);
  }); //seowoo
      //finally
```