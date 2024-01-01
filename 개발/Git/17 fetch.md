`git fetch`는 **동업자가 새로 push한 커밋이 있는지 받아오는 역할**을 한다

```Bash
git fetch 
```

fetch를 하면 변화는 없지만 `git status`를 입력하면 **몇개의 커밋이 뒤쳐져 있는지** 나온다

```Bash
git status 
```

```Bash
git fetch&&git status
```

새로운 브랜치가 있다면 브랜치도 보여준다.

==(이건 git status를 하지 않아도 된다.)==

만약 뒤처져 있다면

```Bash
git pull
```

을 하거나

```Bash
git merge FETCH_HEAD
```

를 하면 된다

---

```Bash
git fe
```

=

```Bash
git fetch&&git status
```