## alias 만들기

alias란 무슨 명령어를 입력하면 무슨 명령어를 실행한다 라는거다.

```Bash
alias python=python3.9
```

python을 입력하면 python3.9를 실행한다는 뜻이다.

띄어쓰기가 있다면 ""로 감싸면 된다

```Bash
alias 띄어쓰기="띄어쓰기"
alias "띄어 쓰기"="띄어 쓰기"
```

이는 zshrc파일에서 만들수도 있다

매번 alias 명령으로 alias을 만드는 것은 번거롭기 때문에 보통은 .zshrc 또는 .bashrc 또는 .bash_aliases 파일에 등록을 해서 사용합니다.