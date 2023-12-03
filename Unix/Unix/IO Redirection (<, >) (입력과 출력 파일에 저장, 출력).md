# IO Redirection (<, >) (입력과 출력 파일에 저장, 출력)

## >

IO Redirection 이란 입,출력의 결과를 파일로 저장하거나 파일에서 명령어를 가져오는 겄이다.

```bash
ls  > result.txt
```

이런 식으로 하면 결과가 출력되지 않고 ls의 결과가 result.txt에 입력된다.

(출력이 없으면 아무것도 기록되지 않는다.)

```bash
touch test1234.txt > test123.txt
```

하지만 오류가 나면 기록되지 않는데

왜냐하면 사실 >앞에는 1이 생략되어 있는데 오류 메시지를 저장하려면 >앞에 2를 붙어서

```bash
rm 1234567890000h-0987654321234567890.txt 2> error.log
```

실제로 파일을 지우면 안될 때도 있어서 일부로 이상한 파일 이름으로 했다.

```bash
rm 12345678987654321h 1> result.txt 2 >error.log
rm 12345678987654321h>result.txt 2>error.log
```

실제로 파일을 지우면 안될 때도 있어서 일부로 이상한 파일 이름으로 했다.

결과) error.log 파일에 

```
rm: cannot remove '12345678987654321h': No such file or directory
```

라는 문장이 적힌다

tip) 띄어쓰기는 상관없다.

## <

<은 파일의 내용을 화면에 출력한다고 보면된다.

```bash
cat < hello.txt
```

hello.txt의 내용이 hi면 hi를 출력한다.

cat hello.txt와 cat < hello.txt의 차이점은 cat hello.txt 는 hello.txt를 인자로 받는거고 cat < hello.txt는 표준 입력이라는 차이점이 있다.

어렵고 잘 사용되지 않아서 그냥 cat hello.txt를 쓰자. 

```bash
head -n1 < head.txt
```

이렇게 적으면 -n1은 인자이고 head.txt는 표준 입력이다.

```bash
head -n1 < head.txt >result.txt&&cat result.txt
```

최종적으로 이렇게 하면 head.txt의 가장 첮줄이 result.txt로 출력이 된다.

그리고 다시 result.txt의 내용이 출력된다.

그리고 기본적으로 내용은 덮어쓰기가 된다.

## >>

이렇게 하면 결과가 추가되는 것이 아닌 추가가 된다.

```bash
ls  >> result.txt
```

## <<

여러줄을 출력할때 사용되고 뒤에나오는내용을 입력하면 여러줄 입력이 멈춘다.

```bash
cat << 1234
```

를 하고 [1>Enter > 2>Enter 3>Enter > 1234>Enter을 누르면 

```
1
2
3
```

이 나온다

```bash

```