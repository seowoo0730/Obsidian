- [ ] Python
- [ ] 프로그래밍 공부
- [ ] 구조 설계
- [ ] REST API
- [ ] Git
- [ ] Git flow
- [ ] Github

# 구조
1. 백테스트
	1. 거래량 상위 종목 찾기
	2. 백테스트 데이터 다운로드
	3. 전략 리스트 받기
	2. 백테스트 실행, 저장
	3. 수익, 거래 횟수 가져오기
	4. 상위 전략 선정
2. 1차 Dryrun
	1. Dryrun용 파일 생성
	2. Dryrun 실행
	4. 수익, 거래 횟수 가져오기(REST API)
	5. 상위 전략 선정
3. Hyperopt
	1. roi
	2. stoploss
	3. trailing stoploss
4. 실거래 실행
#자동매매