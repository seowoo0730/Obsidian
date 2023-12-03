# search (설치할수 있는 프로그램 검색)

```bash
sudo apt-cache search program1
```

program1이라는 이름의 프로그램을 찾는다.

(물론 실제로 없다)

```bash
sudo apt-cache search htop
```

htop이라 는 프로그램을 검색한다 

(이건 있다😆)

그럼 검색 결과로

프로그램이름 - 설~~~~~~명

으로 나온다 그럼 

```bash
sudo apt-get install htop
```

으로 설치하면 된다.

## tip) apt

```bash
sudo apt search program1
```

```bash
sudo apt search htop
```

프로그램이름/설~~~~~~명

```bash
sudo apt install htop
```