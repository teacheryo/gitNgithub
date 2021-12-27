# gitNgithub
헤헤헤
hahaha
#############
ㅁ 깃 설치
1. 구글에서 깃 다운로드 검색

2. git-scm.com 연결

3. git 다운로드 및 설치(next만)

3-1. 환경 설정 및 내용 확인
      -git 설치 직후 전역 환경 설정
        git config --global user.name "ca"
        git config --global user.email "ca1234@naver.com"
       git config --list(환경설정 내용 확인)
   
3-2. 만약 환경설정 중 오타가 발생했을 경우(예: user.name -> usr.name으로 오타 발생 시)
   - usr.name 삭제: git config --global --unset usr.name "ca"
   - user.name 생성: git config --global user.name "ca"

4. c에 폴더 생성 gitworkspace

5. ex01 폴더 추가 생성

6. ex01 안에서 마우스 우클릭 git bash here 선택

7. ls (리눅스 명령어)
====

ㅁ 깃허브 가입
1. sigin up클릭
2. 이메일과 비밀번호 그리고 유저네일 입력 후 y 엔터, 인간임을 확인하는 과정
3. 이메일 확인 및 인증번호 입력
4. 설문에 체크
5. 유료/무료 선택
6. 우측상단의 +를 눌러 new repository 선택하여 ex01 프로젝트 생성
====
자격증명관리자에서 github 증명서 제거


====
ㅁ 소규모 협업하기
1. 팀장이 깃허브에 레파지토리 생성(readme.md 꼭 생성) SMS
2. 팀장은 프로젝트 셋팅을 팀원들에게 제공함
    - 팀장의 로컬 pc의 gitworkspace로 이동
    - git clone SMS 주소
    - 해당 폴더에 가서 마우스 우클리 깃 배쉬 히어를 선택
     - touch 환경설정.txt하여 파일 생성
     -git add.
     - git commit -m "환경설정 완료"
     - dev브런치생성: git checkout -b dev
     - 최초에 한해서 main, dev 브랜치의 내용을 깃허브에 올린다.
        git push --all
     - git hub를 보면, 로컬에 있던 브랜치가 추가된 것을 확인할 수 있음.
     - github의 SMS레파지토리를 선택한 후,setting을 한다.
     - 셋팅의 branches를 통해 팀원들이 배포브랜치인 main, 개발브랜치인dev에 push하지 못하도록 막는다.(add rule 버튼을 두 번)
     - 셋팅의manage access를 통해 팀원들이 해당 레파지토리에 브랜치를 만들 고 git push할수 있도록 한다.   
  - 셋팅의manage access를 통해 팀원들에게 초대장 발송(콜라보레이션)
     - 팀원들은 기능에 맞는 각각의 feature 브랜치들을 만들어 작업 후 push
     
3. 팀원들은 특정 폴더 안에서 마우스 우클릭 깃 배쉬 히어 선택
   git clone sms 레파지토리 주소
4. git log를 통해 현재 상태 확인
5. git branch를 통해 현재 가지고 있는 브랜치 확인 및 작업 브랜치 확인
6. git checkout -b dev origin/dev
   - dev 브랜치 생성 및 작업 브랜치로 지정 그리고 github에서 내려받은
     dev 브랜치의 내용과 merge한다.
7. 작업 브랜치 생성(feature/join: 회원 가입 브랜치) 후 이 브랜치를 작업브랜치로 설정
   - git checkout -b feature/join

8. touch 회원가입.txt(회원가입 텍스파일 생성)

9. git add .
10. git commit -m "회원가입 완료"

11. git push origin feature/join : 깃허브의 feature/join 브랜치에 push
    - 만약 github에 feature/join 브랜치가 없으면 자동 생성됨.

12. 팀장의 깃허브에 접속하여 PR 요청
     - 해당 레파지토리에 들어가서 레파지토리 이름 아래의 탭 메뉴 중 [Pull requests]메뉴를 클릭
     - 바뀐 화면에서 우측의 초록생 버튼 중 [New Pull Requests] 선택
     - dev <- feature/join이 되도록 브랜치를 선택
     - 바로 한 줄 밑의 우측에 있는 초록색 버튼인 [Create pull request] 클릭
     - 입력창에 코멘트를 남기고 하단의 초록생 버튼인 [Create pull request]를 클릭

13. x Revie required, x Merging is blocked가 빨간색으로 나옴.

14. 팀장이 깃허브에 로그인한다.
15. 해당 레파지토리에 들어가서 레파지토리 이름 아래의 탭 메뉴 중 [Pull requests]메뉴에 PR 요청이 몇 건이 있는지 숫자가 적혀 있음. 클릭

16. 코멘트 클릭
17. 전환된 화면의 첫 번째 탭인 [Conversation]탭을 통해 내용 확인
18. 같은 화면의 끝에 있는 [Files change]탭을 통해서 변경된 파일 확인
19. 같은 화면의 두 번째 탭인 [Commits]탭을 통해서 커밋 내용 확인 후 클릭

20. 전환된 화면의 우측에 초록색 버튼인 [Review changes]를 클릭하면, 숨겨진 화면이 열림.
21. 해당 화면에 조언/승인/거절을 라디오버튼으로 선택하고 하단의 초록색 [submit review] 버튼을 클릭

22. 전환된 화면에서 초록색의 [Merge pull requests]를 클릭

23. 전환된 화면에서 초록색의[Confirm merge] 버튼 클릭

24. 같은 팀원들에게 이 내용을 전달함.

23. 해당 팀원은 팀장의 레파지토리에 등록된 feature/join 브랜치를 삭제
- git push --delete origin feature/join

24. 해당 팀원은 자신이 갖고 있는 브랜치를 삭제해도 되지만 가지고 있는 것을 추천함. 삭제하고 싶다면
  git branch -d feature/join

25. 다른 팀원들은 해당 기능을 dev 브랜치 pull한다. 
- git checkout dev
- git pull origin dev

26. 그리고 각자가 작업하는 브랜치에서 commit이 끝나면,  rebase를 해서 해당 기능을 추가한다
- git checkout feature/list
- git add .
- git commit -m "목록조회 끝"
- git rebase dev

27. merge도 하나의 commit으로 인식하게 하고 싶으면
git merge --no--ff 작업 브랜치

28. 만약pr이 거절당한 후라면
git push -f origin 작업 브랜치
이때는pr 요청을 안 함.


 

