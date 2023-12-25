`git merge`를 하면 현재 브랜치에 뒤에 나오는 브랜치를 **병합**(가져오기) 한다

### ***주의 병합을 하기 전에 꼭 병합할 브랜치로 이동하시오!**

```Bash
git merge branch-name
```

현재 브랜치가 master 이면 master에 다른 브랜치 면 다른 현재 브랜치에 병합된다

## 충돌 해결하기

`git merge`를 할 때 같은 파일에 **같은 부분에 수정**을 하고 merge를 하면 충돌이 일어나는데

그럼 충돌을 직접 해결하거나 merge 툴을 이용해서 **충돌을 해결**하고 `git add .`

`git commit`을 하면 자동으로 **병합하는 커밋**이라고 입력이 돼있다

### `--no-ff`

**충돌을 해결**할 때 자동으로 커밋이 앞으로 갈 때가 있는데 그러지 않게 해준다

```Bash
git merge --no-ff
```

### merge 툴을 이용해 해결하기

**diff 툴을 이용해 비교**하려면 diff 다음에 tool을 붙이면 설정한 **diff 툴**로 열린다(설정은 config로)

```Bash
git mergetool
```

---

```Bash
git mer
```

  

```Bash
git mt
```

=

```Bash
git mergetool
```