`git push`를 하면 **현재 정보가 연결된 저장소로 간다**

```Bash
git push
```

*주의 [[원격 저장소 연결하기]] 실행

그리고 push를 할 때는 **비밀번호를 입**력하면 된다

*주의 모든 커밋을 pull 하기 전에는 push를 할 수 없다==(만약 하지 않았다면 pull 한 다음에 충돌을 해결하고 add, commit, push 하면 된다)==

```Bash
git pull
```

## `-u`

 `-u` 명령어는 **한 번만 원격 저장소 이름과 브랜치 이름을 입력하고 그 이후에는 모든 저장소 이름과 브랜치 이름을 생략**할 수 있다

```Bash
git push -u origin master
```

원래는 이렇게 해야한다

```Bash
git push (원격-이름) (브랜치-이름)
```

```Bash
git push origin master
```

예시이다 ==(다를 수 있음)==

### `--tags`

`--tags` 명령어는 저장소의 **모든 tag를 원격 저장소에** `push` 하는 명령어이다

```Bash
git  push --tags
```

한번 미리 연결했으면 하지 않아도 된다==(git push만 하면 된다)==

---

```Bash
git config --global push.default current
```

이렇게 설정하면 한 번도 `-u`를 하지 않아도 된다

---

```Bash
git ps
```