`git status`를 하면 현재 폴더의 **파일들의 상태**를 보여준다

```Bash
git status
```

==빨간색==이면 add가 안 된 상태 ==파란색==이면 add는 된 상태 다 commit을 하면 nothing to commit, working tree clean이라고 나온다

  

파일 내용이 변경됐는데 add가 안 됐었으면

==modified: 파일명==

  

파일이 삭제되면

deleted: ==파일명==

  

한 번도 add가 안됐었으면

(use "git add <file>..." to include in what will be committed)  
파일명  

등등으로 나온다.

`-s`를 붙이면 간단하게 나온다

---

```Bash
git s
```