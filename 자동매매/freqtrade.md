### [freqtrade](https://www.freqtrade.io/en/stable/)
### [freqtrade github](https://github.com/freqtrade/freqtrade)

### Using Freqtrade with Docker
``` zsh
mkdir ft_userdata
cd ft_userdata/

# Download the docker-compose file from the repository
curl https://raw.githubusercontent.com/freqtrade/freqtrade/stable/docker-compose.yml -o docker-compose.yml

# Pull the freqtrade image
docker compose pull

# Create user directory structure
docker compose run --rm freqtrade create-userdir --userdir user_data

# Create configuration - Requires answering interactive questions
docker compose run --rm freqtrade new-config --config user_data/config.json
```
### docker로 freqtrade 업데이트
``` zsh
# Download the latest image
docker compose pull

# Restart the image
docker compose up -d # -d 백그라운드 에서 실행
```
>[!warning]
>변경 사항/수동 개입이 필요한지 항상 변경 로그를 확인하고 업데이트 후 봇이 올바르게 시작되는지 확인해야 한다.
### Adding a custom strategy
`user_data/strategies/`에서 전략 복사
`docker-compose.yml`파일에 전략 클래스 이름 추가

### 봇 시작
```zsh
docker compose up -d # -d 백그라운드 에서 실행
```
거래 모드를 시작한다. docker 답변에 따라 테스트 실행 또는 실시간 거래
>[!Warning]
>기본 구성
>봇을 시작하기 전에 모든 옵션이 원하는 항목(예: 가격 책정, 쌍 목록 등)과 일치하는지 확인해야 한다.
### 봇 모니터링
``` zsh
docker compose ps
```
로그확인
`docker compose logs -f` 혹은 `user_data/logs/freqtrade.log`에서 찾기

데이터베이스
`user_data/tradesv3.sqlite`
### freqUI
`http://0.0.0.0:8080/`로 접속하기
### freqtrade 실행
``` zsh
docker compose run --rm freqtrade <command> <optional arguments> # --rm 포함하면 완료 후 컨테이너가 제거되며 거래 모드(freqtrade trade명령으로 실행)를 제외한 모든 모드에 적극 권장된다.
```
### docker추가 종속성
전략에 기본 이미지(docker)에 포함되지 않은 종속성이 필요한 경우 호스트에 이미지를 빌드해야 한다
`docker-compose.yml` 에서 build 주석 제거 및 이름 바꾸기
``` zsh
image: freqtrade_custom
build:
	context: .
	dockerfile: "./Dockerfile.<yourextension>"

```
`docker compose build --pull` 실행