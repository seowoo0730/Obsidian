`git tag`는 tag란 말 그대로 **코드상에서 책갈피** 역할을 해주는 기능이다

**일반적으로는 출시를 할 때 사용**한다

```Bash
git tag
```

`git tag` 명령어는 tag를 확인할 때 사용된다

## tag 만들기

### lightweight tag

lightweight tag는 tag 이름만 정할 수 있는 tag이다

```Bash
git tag (tag-이름)
```

```Bash
git tag v1.0.0
```

## annotated tag

annotated tag는 여러 설명을 적을 수 있는 tag이다

```Bash
git tag -a (tag-이름)
```

```Bash
git tag -a v2.0.0
```

```Bash
git tag -a (tag-이름) -m "(tag 메시지)"
```

```Bash
git tag -a v2.0.0 -m "2021-5-8"
```

## `-d`

`-d` 명령어는 tag를 삭제하는 명령어이다

```Bash
git tag -d (tag-이름)
```

```Bash
git tag -d v1.0.1
```

### 원격 저장소 tag 지우기

그냥 tag를 지우면 원격 저장소의 tag는 지워지지 않는데

뒤에 원격 저장소 이름을 적으면 된다

```Bash
git tag -d (원격-저장소-이름) (tag-이름)
```

```Bash
git tag -d origin v1.0.0
```

## 전 버전에 tag 만들기

```Bash
git tag (tag-이름) (커밋-아이디)
```

```Bash
git tag v1.0.0 a1b2c3
```