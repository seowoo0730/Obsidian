**git flow란 브랜치를 사용하는 방법의 사례 또는 사례를 쉽게 운영할 수 있는** [[git flow(프로그램)]]을 이다

![[개발/Git/img/Untitled 6.png|Untitled 6.png]]

### master과 develop을 제외한 모든 커밋은 병합 후 삭제해야 한다

==모든 브랜치는 병합할 때 --no-ff를 추가해야 한다==

## master

master 브랜치는 기본 브랜치로 언제나 실행 가능한 상태여야 한다 ==(오류가 없어야 함)==

release 브랜치만 master 브랜치에 병합될 수 있다

==(하위 브랜치 없음)==

==hotfix, release 브랜치만 master 브랜치에 병합될 수 있다==

## develop

실제 개발을 하는 브랜치이다

develop 브랜치만 release 브랜치에 병합될 수 있다

==(하위 브랜치 없음)==

## release/

release 브랜치는 출시를 준비하는 브랜치이다 ==(오류 수정만 한다)==

release 브랜치는 release/버전명으로 하위 브랜치가 있어야 한다

develop 브랜치만 release 브랜치에 병합될 수 있다

==hotfix, release 브랜치만 master 브랜치에 병합될 수 있다==

==(하위 브랜치가 있어야 함)==

==(지속적으로 커밋을 만들 때마다 develop 브랜치에 병합해야 한다)==

==(develop 브랜치로부터 생성됨)==

## feature/

feature 브랜치는 기능을 개발하는 브랜치로 기능마다 하위 브랜치를 만든다

feature 브랜치는 feature/기능명으로 하위 브랜치가 있어야 한다

==(하위 브랜치가 있어야 함)==

==(지속적으로 커밋을 만들 때마다 develop 브랜치에 병합해야 한다)==

## hotfix/

hotfix 브랜치는 ==**긴급**==하게 master 브랜치에 수정할 내용이 생겼을 때 사용되는 브랜치이다

hotfix 브랜치는 hotfix/버전명으로 하위 브랜치가 있어야 한다

==(하위 브랜치가 있어야 함)==

==(master 브랜치로부터 생성됨)==

==(수정을 완료하면 master 브랜치에 병합해야 한다)==

[[git flow(프로그램)]]