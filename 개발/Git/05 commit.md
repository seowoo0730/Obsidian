지금까지 add된 파일의 **버전을 만드는 것**이다

```Bash
git commit
```

## `-m`

뒤에 **커밋 메시지**를 적는다

```Bash
git commit -m "설명 ~~~  ~~"
```

**-m**을 안 붙이면 [[01 config]]가 나오고 설명을

써야 한다

```Bash
git commit
```

그럼 앞에 커밋 아이디 7자리가 출력된다

## `-a`

`-a`를 붙이면 staging area에 파일을 모둔 **add 후 commit** 한다

```Bash
git commit -a
```

아직 추적 중이지 않은 파일 ==(add된 적 없는 파일)==은 커밋 되지 않는다

### 둘을 합치면(-a, -m)

```Bash
git commit -am "설명 ~~~~~ ~~"
```

```Bash
git commit -am "commit"
```

==(커밋은 작은 단위로 나눠 해야 한다)==

## `--amend`

`--amend`는 **최근 작업을 전 커밋에 포함** 시켜준다

```Bash
git commit --amend
```

## git commit message 작성법

> [!info] Git 커밋 메시지 작성법  
> 프로젝트가 지루하게 늘어지면, 커밋 메시지는 점점 더 무의미해진다.  
> [https://item4.blog/2016-10-31/How-to-Write-a-Git-Commit-Message/](https://item4.blog/2016-10-31/How-to-Write-a-Git-Commit-Message/)  

---

```Bash
git c
```

  

```Bash
git ac
```

=

```Bash
git add . && git commit
```

  

```Bash
git acm
```

=

```Bash
git add . && git commit -m
```

==(뒤에 띄어 쓴 후 ""안에 커밋 메시지를 적으면 된다)==