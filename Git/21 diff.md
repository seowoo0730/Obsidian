**git에 전 버전**(staging area 또는 전 커밋)**과 비교**하는 것이다

그리고 ==+==는 추가 삭제는 ==-==로 나온다

```Bash
git diff
```

## staging area 파일 비교하기

그냥 diff는 현재 working directory에 있는 파일만 비교하는데 **staging area에 파일을 비교**하려면

```Bash
git diff --staged
```

를 붙이면 된다.

## diff 툴을 이용해 비교하기

diff 툴을 이용해 비교하려면 diff 다음에 tool을 붙이면 설정한 diff 툴로 열린다

```Bash
git difftool
```

---

```Bash
git d
```

```Bash
git dt
```