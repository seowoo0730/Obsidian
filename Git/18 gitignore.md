git으로 관리되거나 굳이 **github에 올릴 필요가 없는 내용**은 (실행하면 패키지가 다운로드해지는 코드, 코드대로 빌드 돼서 자동으로 생성되는 파일들, 보안적으로 중요한 내용)

**.gitignore을 이용해 git의 관리에서 제외**할 수 있는데 프로젝트 폴더 바로 안 폴더에 .gitignore이라는 폴더를 만들고 그 파일 안에 제외할 파일 이름을 적으면 된다

그럼 git add를 하지 않아도 git status에 나오지 않는다

> [!info] .gitignore file - ignoring files in Git | Atlassian Git Tutorial  
> Git sees every file in your working copy as one of three things: tracked - a file which has been previously staged or committed; untracked - a file which has not been staged or committed; or ignored - a file which Git has been explicitly told to ignore.  
> [https://www.atlassian.com/git/tutorials/saving-changes/gitignore](https://www.atlassian.com/git/tutorials/saving-changes/gitignore)  

여기를 참조하자

.gitignore을 사용할때 *을 사용할수도 있고

만약 한 폴더안에 모든 파일을 제외하고 싶을때는

```Plain
(폴더)/
```

```Plain
build/
```

을 사용하면 된다

그리고 서로 합쳐서

```Plain
build/*.log
```

처럼 사용할수 있다.

build폴더 안에 모든.log파일을 제외한다.