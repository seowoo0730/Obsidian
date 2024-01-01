**Git**은 **버전 관리 도구**(VCS) 중에 하나이다

## 설치

### linux

```Bash
sudo apt install git
```

---

### window

> [!info] Downloading Git  
> You are downloading the latest ( 2.  
> [https://git-scm.com/download/win](https://git-scm.com/download/win)  

  

![[개발/Git/img/Untitled 1.png]]

---

### `git`

`git` 명령어는 git의 **명령어**들 과 **사용법**을 알려준다

```Bash
git
```

---

### `-version`

`git --version`은 git의 **버전**을 알려준다

```Bash
git --version
```

---

git을 사용하지 않으려면 **.git** **폴더**를 **삭제**하면 된다

---

모든 명령어 뒤에 **--h**를 붙이면 **설명**이 나온다

---

### 파일 선택

파일을 선택할 때 `*`이라고 하면 **모든 파일**에 명령어를 실행한다.

```Bash
git (명령어) *
```

```Bash
git add *
```

---

`*`을 **앞**에 넣으면 뒤에 맨 **뒤에** ~~가 **포함**된 파일을 모두 명령어를 실행한다

```Bash
git (명령어) *(~~)
```

```Bash
git add *.txt
```

**모든** `.txt` 확장자 파일을 add 한다

---

**앞**에 ~~가 **포함**된 파일을 **모두** 명령어를 실행한다

```Bash
git (명령어) (~~)*
```

```Bash
git add a*
```

라고 하면 모든 .a가 맨 앞에 있는 파일을 add한다

이건 .gitignore을 작성할 때도 쓰인다

[[config]]

[[init]]

[[add]]

[[status]]

[[commit]]

[[log]]

[[revert]]

[[reset]]

[[checkout (이동)]]

[[branch (브랜치)]]

[[merge (브랜치 병합)]]

[[rebase]]

[[remote (저장소)]]

[[원격 저장소 연결하기]]

[[push]]

[[pull]]

[[fetch]]

[[gitignore]]

[[clone]]

[[rm]]

[[diff]]

[[cherry-pick]]

[[stash]]

[[tag]]

[[git flow]]

[[work flow (작업환경)]]