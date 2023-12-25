`git cherry-pick`은 **다른 브랜치의 버전을 현재 브랜치에 생성하는 명령어**이다

원래의 추가할 버전의 전체가 아닌 그 버전의 변화만을 가져오는 기능이다

### ***주의 cherry-pick을 하기 전에 꼭 병합할 브랜치로 이동해야 한다**

```Bash
git cherry-pick (병합될-버전-번호)
```

```Bash
git cherry-pick a1b2c3
```

을 하면

a1b2c3에 해당하는 버전이 현재 브랜치 앞에 생긴다