`git remote`는 git에 **원격 저장소를 연결하고 확인하는 명령어**이다

```Bash
git remote
```

를 입력하면 현재 연결 중인 저장소 이름이 나온다

## -v

만약 저장소가 아니라 주소를 보고 싶다면 -v를 붙이면 된다.

```Bash
git remote -v 
```

## 원격 저장소 연결하기

git remote add 뒤에 저장소 이름과 주소를 적으면 저장소가 연결된다.

```Bash
git remote add origin https://~~~~~/~~~~/~~~
```

저장소의 기본 이름은 origin이다