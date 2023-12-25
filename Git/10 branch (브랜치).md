## 브랜치 목록 보기

`git branch`를 입력하면 **브랜치들의 이름들과 현재 브랜치**를 보여준다

```Bash
git branch
```

현재 브랜치는 앞에 * 이 붙어있고 ==초록색==이다

**q**를 눌러 나올 수 있다

## 새로운 브랜치 만들기

```Bash
git branch branch-name
```

새로 나온 브랜치는 원래 자신이 생성된 브랜치와 상태가 같다

==(브랜치는 /를 이용해 폴더 구조처럼 만들 수 있다)==

```Bash
git branch feature/login
```

## 브랜치 삭제하기

브랜치를 **삭제**할 때는

(로컬 (내 컴퓨터)의 내용만 볼 수 있다)

```Bash
git branch -D branch-name
```

**-d**의 **대소문자는 상관없다**

### 원격 브랜치 삭제하기

원격 브랜치를 **삭제**할 때는

을 입력하면 된다

```Bash
git branch -d origin remote-branch-name
```

## 브랜치를 만들고 바로 이동

브랜치를 **만들고 바로 이동**할 때는

```Bash
git checkout -b branch-name
```

을 하면 된다

## 원격 브랜치도 보기

**원격 브랜치의 목록**도 보려면

```Bash
git branch -a
```

를 하면 된다

작동을 하려면 [[17 fetch]]를 해야 한다

```Bash
git fetch
```

## 원격 브랜치 가져오기

```Bash
git checkout -b (만들-브랜치-이름) (원격)
```

---

```Bash
git br
```