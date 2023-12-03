# 패키지 매니저 (apt-get, apt-cache, sudo apt)

apt -get은 패키지 매니저중 하나로 프로그램을 설치, 삭제, 등등..을  할수 있게 해준다.

설명을 보려면 

```bash
sudo apt-get
sudo apt
sudo apt-cache
```

처럼 패키지 매니져 이름만 입력하면 된다

apt-get을 사용하기 전에는

```bash
sudo apt-get update&&sudo apt-get upgrade
sudo apt update&&sudo apt upgrade
```

를 하면 된다.

## tip) apt-get vs apt

apt는 apt-get과 apt-cache의 기능 중에서 잘 사용되지 않는 기능을 제외하고 만든 새로운 tool이다.

여기서 apt-get은 패키지 설치를 담당하고, apt-cache는 패키지 검색을 담당하는 tool이다.

결론적으로 apt-get이 아닌 apt를 사용하는 것이 사용성 측면에서는 유리하다.

apt는 조금더 apt-get이나 apt-cache보다 조금더 Gui에 가깝고 예쁘다. + 더많은 정보를 준다.

굳이 apt-get이나 apt -cache를 쓸 이유가 없다면 apt를 사용하자 apt-get기준으로 사전을 정리하지만 뒤에 tip) apt로 apt로 사용법도 적어 놓겠다

[upgrade (패키지 업그래이드)](upgrade%20(패키지%20업그래이드).md)

[update (패키지 업데이트)](update%20(패키지%20업데이트).md)

[downlaod (install)하는법](downlaod%20(install)하는법.md)

[search (설치할수 있는 프로그램 검색)](search%20(설치할수%20있는%20프로그램%20검색).md)