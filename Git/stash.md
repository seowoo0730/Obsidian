git에서는 **현재 작업 중일 때 커밋을 하지 않으면 다른 브랜치로 checkou**t 할 수 없는데 할 수 있게 해주는 명령어가 `git stash save`이다

```Bash
git stash save
```

(git stash만 입력해도 된다)

```Bash
git stash
```

(git stash는 추적 되고 있는 파일에만 가능하다)

`git stash`를 하면 수정했던 내용이 잠시 사라지는데 다시 전에 작업 중이던 브랜치에 돌아와서 git `stash apply`를 하면 된다

```Bash
git stash apply
```

git stash의 목록을 보려면 `git stash list`를 하면 된다

```Bash
git stash list
```

`git stash save`를 하면 `git stsah list`에 남아 나중에 적용할 수 있는데 가장 최근 stash save 한 것부터 적용하려면 `git stash apply` 후 `git stash drop`을 하면 가장 최근 stash가 stash list에서 삭제된다

```Bash
git stash drop
```

그리고 다시 `git stash apply`를 해 적용하면 된다

그리고 이처럼 `git stash apply`와 `git stash drop`을 **동시에** 할 수 있는데 `git stash pop`을 하면 된다

```Bash
git stash pop
```

---

```Bash
git ss
```

```Bash
git sp
```

```Bash
git sl
```

```Bash
git sd
```

```Bash
git sp
```