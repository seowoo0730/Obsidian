**다른 버전으로 이동**하기

예전 버전으로 돌아가려면

```Bash
git checkout (번호)
```

```Bash
git checkout a1b2c3
```

을 하면 된다.

만약 돌아갈 버전에 브랜치가 2개 이상 있다면 번호가 아닌 **브랜치**로 이동해야 한다

다시 **최신 버전**으로 가려면

```Bash
git checkout (브랜치-이름)
```

```Bash
git checkout master
```

을 하면 된다

(2번째는 예시이고 다를수 있다)

## 다른 브랜치로 이동하기

다른 브랜치로 이동할 때는 현재 위치(커밋)을 바꾸는 것처럼

```Bash
git checkout (브랜치-이름)
```

```Bash
git checkout branch-name
```

을 입력하면 된다

## 브랜치를 만들고 바로이동

브랜치를 만들고 바로 이동할때는

```Bash
git checkout -b (브랜치명) 
```

```Bash
git checkout -b branch-name
```

을 하면 된다

---

```Bash
git ch
```