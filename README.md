# TypeScript 템플릿 By OKTROCO

- 타입스크립트 기반으로 작업을 하기 위한 기본 템플릿
- eslint, prettier, gitignore설정이 되어있다
- 용도별로 꾸며서 쓰면된다
- 자주 이용하는 용도는 환경구축 코드를 ShellScript로 작성할 예정

## 용도별 사용법

### React (CRA)

- CRA.sh 실행

  ```shell
  bash CRA <AppName>
  ```

### 그 외

- 알아서 입맛에 맞추면 됨


# (추천) 피클플러스의 readme

# 기본 숙지사항

- 그냥 코드 == 기계가 읽기 쉬운 코드
- 좋은 코드 == 사람이 읽기 쉬운 코드
- 좋은 코드를 짜기 위해 머리 아픈 시간 < 급한 코드로 나중에 머리 아픈 시간

# 협업 가이드

- PR을 올릴 때는 yarn format(prettier) && yarn fix(eslint) 진행
- PR을 올리면 yarn prettier, yarn lint, yarn test 진행 후, 통과 못하면 PR이 Closed처리됨
- PR은 upstream의 dev, 혹은 상위 feature브랜치로 올리는 것이 원칙
- PR할 때 올리는 branch에 commit 수는 1개, commit을 하며 작업을 진행하되 올리기전 rebase -i로 스쿼시한다
- 스쿼시 되는 모든 커밋은 commit message의 내용부분으로 들어가고 제목은 jira티켓아이디와 task내용을 적는다
- PR후 피드백 적용 코드 또한 rebase -i 로 스쿼시해서 한개의 commit으로 합친다

### 커밋메시지 예시 (내용은 행 앞에 - 를 적고 제목은 <jira이슈키>: <제목> 형태로 한다)

```
PKW-51: Notice 컴포넌트, 컨테이너 제작

- 함수형 컴포넌트로 전환, Header 컨테이너 컴포넌트 분리
- div 기본 스타일 실수 수정, #root에 justify_content=center 설정
- 뒤로가기 아이콘 컴포넌트 추가
- DesktopModalPositon interface 추가, 마이페이지, 알림창 전용
- 알림 관련 redux slice 작성
- Notice Presentation Component 완성
- Notice 상태관리 컨테이너 추가
- 헤더에 Notice추가 임시코드 작성
- Notice 컴포넌트 테스트스크립트 작성
- Notice의 모바일/데탑 대응을 display속성으로 조절
```

# PicklePlus 개발관련 문서들

[프론트엔드 리팩토링 문서](https://www.notion.so/723d25262c2b48ab80a34d153dfc5487)<br>
[좋은 코드, Clean Code](https://www.notion.so/Clean-Code-7953884db77440adaa4e3798fd7ed98b)
