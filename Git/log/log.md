지금까지 만든 **커밋들의 정보** ==(이름, 일련번호)==을 보여준다

```Bash
git log
```

q를 눌러 나올 수 있다.

## HEAD

HEAD란 지금 내가 어떤 브랜치, 버전에 있는지 알려준다

**HEAD가 향한 곳이 현재 위치**이다

![[/Untitled 2.png|Untitled 2.png]]

## `--graph`

**시각화된 log**를 보여준다

```Bash
git log --grag
```

## `-- all`

`--all`은 모든 브랜치를 보여준다

```Bash
git log --all
```

## `--decorate`

`--decorate`는 쉽게 브랜치가 어떤 커밋을 가리키는지 확인할 수 있다

```Bash
git log --decorate
```

## `--oneline`

`--online`을 사용하면 log를 작게 보여준다

```Bash
git log --one line
```

## 모든 브랜치 예쁘게 시각화된 짧은 log 보기

```Bash
git log --graph --all --decorate --oneline
```

예쁘게 시각화된 git log를 볼 수 있다

## `--stat`

각 버전마다 있는 파일, 정보 ==(추가, 삭제한 줄)==를 알려준다

```Bash
git log --stat
```

## `-p`

버전들을 비교하면서 볼 수 있다

```Bash
git log -p
```

---

```Bash
git l
```

=

```Bash
git log --color --graph --decorate --all  --oneline  --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr)%C(bold blue)<%an>%Creset' --abbrev-commit
```