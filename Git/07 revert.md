`git revert`는 **과거의 시점을 복원한 커밋**을 만든다고 생각하면 되는데

과거로 돌아가는 거는 `reset`과 같지만 **과거의 시점과 같은 커밋을 새로 만든다**고 생각하면 된다

`git reset`과 마찬가지로 `git log`를 해서 나온 커밋 뒤에 **일련번호를 복사 후** `revert` **뒤에 붙여 넣으면 된다**

revert는 reset과 다르게 뒤에 나오는 일련번호의 커밋을 되돌리는 거다

```Bash
git revert (번호)
```

```Bash
git revert a1b2c3
```

그러면 **커밋 메시지 작성 화면**이 나오는데 그럼

작성하면 된다

**여러 커밋을 되돌릴 때는 바로 직전 커밋부터 전전 커밋 전 전 전 커밋처럼 역순으로 차례차례 입력**해야 한다.

만약 커밋 4까지를 되돌리고 싶은데 커밋이 7까지 있다면 라면 ==(현재 커밋이 7이다)==

7을 되돌리고 6을 되돌리고 5를 되돌리면 된다