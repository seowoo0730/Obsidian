rebase는 merge와 비슷하지만 **브랜치가 한 줄로 연결이 돼서 더욱 깔끔하게 정리**할 수 있다

사용법은 merge와 같다

```Bash
git rebase (브랜치-이름)
```

```Bash
git rebase branch-name
```

## 충돌 해결하기

```Bash
git am --show-current-patch
```

을 하면 충돌이 생긴 지점을 보여준다

그리고 [[11 merge (브랜치 병합)]]처럼 충돌을 해결하면 된다

그리고

```Bash
git rebse --continue
```

를 하면 된다

만약 또 충돌이 나면 다시

그리고 [[11 merge (브랜치 병합)]]처럼 충돌을 해결하면 된다

그리고 또 `git rebase --continue`를 하면서 진행 하면 된다