pipeline [|]은 |앞에있는 명령어의 출력(결과)값을 | 뒤에있는 명령어의 입력값으로 하다는 명령어와 같다.

```Bash
ls --help | grep sort
```

ls --help를 했을때 출력(결과)값에서 sort 가 들어간 문장을 출력한다.

|는 여러개를 사용해도 된다.

```Bash
ls --help | grep sort | grep file
```

ls --help를 했을때 출력(결과)값에서 sort 가 들어간 문장을 출력한값에서 file이 들어간 값을 출력한다.

띄어쓰기도 상관없다.

```Bash
ls --help| grep sort    |grep file
```