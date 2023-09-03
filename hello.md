# 토큰 생성

- 인증
- 생성한 토큰은 안전한 곳에 보관 (유출 주의)
- 권한 지정 후 토큰 생성 (생성 후 권한 변경 가능)
- 비밀번호 대신 사용
- 토큰
    
    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
    

# 소스트리 사용해보기

**clone → 업로드할 파일 선택, add → commit → push**

### Clone

- 원격 저장소의 내용 → 내 컴퓨터

**Source Tree를 통해 저장소 클론**

- Clone or 복제/생성 메뉴 → github에서 생성한 저장소(Repository) 클론
    
    내 문서 아래 같은 이름의 디렉터리 생성
    

### Add (스테이지에 올리기)

- 커밋하기 전에 저장을 원하는 파일들을 묶는 것 → 커밋

### Commit

- 스테이지에 올라온 파일을 내 컴퓨터에 저장
    
    게임의 세이브 (언제든지 커밋한 시점으로 돌아갈 수 있음)
    
- 저장을 원하는 파일들을 묶어서 커밋 명령 수행

주의 사항

- 반드시 한 번에 하나의 논리적 작업만 커밋
    
    여러 작업 →여러 번 커밋
    
- 커밋 메시지 작성법
    
    첫 줄에 간단하고 명확하게 내용 작성
    
    한 줄 비우고
    
    자세한 내용
    
    영어로 작성하면 더 좋음
    

### Push (Github에 업로드)

- 커밋을 하면 세이브 데이터가 내 컴퓨터에 저장
- github에 업로드 → 공유, 복구 가능

- ❗Source Tree Push 오류
    
    오류 메시지
    
    git -c diff.mnemonicprefix=false -c core.quotepath=false --no-optional-locks push -v --tags origin main:main
    
    remote: Support for password authentication was removed on August 13, 2021.
    
    remote: Please see
    
    https://docs.github.com/en/get-started/getting-started-with-git/about-remote-repositories#cloning-with-https-urls
    
    for information on currently recommended modes of authentication.
    
    fatal: Authentication failed for '
    
    https://github.com/lemonaS2/github_test.git/'
    
    Pushing to
    
    https://github.com/lemonaS2/github_test.git
    
    오류가 나면서 완료됨.
    
    오류 해결
    
    인증 수단으로 비밀번호가 아닌 토큰 이용
    
    [[Git/GitHub] - 소스트리(Sourcetree)에서 push시 토근 인증 요구[remote: Support for password authentication was removed on August 13, 2021.] 오류 해결 방법](https://pingfanzhilu.tistory.com/entry/GitGitHub-소스트리Sourcetree에서-push시-토근-인증-요구remote-Support-for-password-authentication-was-removed-on-August-13-2021-오류-해결-방법)
    
    소스트리 우측 상단 설정 클릭
    
    저장소 설정 → 원격 경로 주소 부분 더블 클릭
    
    URL/경로 부분에 깃허브에서 생성한 “개인토큰@” 추가
    
    (기존: https://github.com/abc/a.git -> 변경: [https://토큰값@github.com/abc/a.git](https://%ED%86%A0%ED%81%B0%EA%B0%92@github.com/abc/a.git))
    

### 코드 뭉치 버리기

- 저장하지 않은 변경 내용 취소하기
- 마지막 커밋(세이브)으로 돌아가기


