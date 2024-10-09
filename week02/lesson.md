# 2주차: 소프트웨어 기본 도구 및 환경 설정 - 강의 내용

# Week 02: 소프트웨어 기본 도구 및 환경 설정 - 강의 내용

### 슬라이드 1: Git의 개념
Git은 분산 버전 관리 시스템으로, 여러 개발자가 동시에 협업할 수 있도록 돕습니다. 각 개발자는 로컬에서 작업을 수행하고, Git을 통해 변경 사항을 공유하며 관리할 수 있습니다.

### 슬라이드 2: 버전 관리의 중요성
버전 관리 시스템(VCS)은 소스 코드 변경 이력을 추적하고, 문제 발생 시 이전 버전으로 쉽게 되돌릴 수 있게 해줍니다. 이 과정에서 협업 효율성을 크게 향상시킬 수 있습니다.

### 슬라이드 3: Git 설치 방법
Windows와 macOS에 Git을 설치하는 방법을 설명합니다. `git-scm.com`에서 Git을 다운로드한 후, 설치 프로그램을 실행하여 Git을 설치할 수 있습니다.
- [Git 설치 가이드](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)

### 슬라이드 4: Git 기본 설정
설치 후 첫 번째로 해야 할 일은 사용자 이름과 이메일 주소를 설정하는 것입니다. 이는 모든 커밋 기록에 반영됩니다.

$ git config --global user.name "Your Name" $ git config --global user.email "your.email@example.com"


### 슬라이드 5: Git 저장소 초기화
프로젝트 폴더에서 Git 저장소를 초기화하여 버전 관리를 시작할 수 있습니다.

$ git init

### 슬라이드 6: GitHub와 연동하기
GitHub는 Git을 활용한 협업을 위한 클라우드 기반 플랫폼입니다. GitHub에서 새 저장소를 생성한 후, 로컬 Git 저장소와 연결할 수 있습니다.

$ git remote add origin https://github.com/your-username/your-repo.git


### 슬라이드 7: 파일을 Git에 추가하기
변경된 파일을 Git에 추가하는 방법입니다. 파일을 추적하도록 추가하려면 `git add` 명령어를 사용합니다.

$ git add .


### 슬라이드 8: 커밋하기
Git 커밋은 변경 사항을 로컬 저장소에 저장하는 것을 의미합니다. 커밋 메시지를 작성하여 변경 내용을 설명합니다.

$ git commit -m "Initial commit"


### 슬라이드 9: GitHub에 푸시하기
GitHub와 연동된 원격 저장소에 변경 사항을 푸시하여 공유할 수 있습니다.

$ git push origin main


### 슬라이드 10: 기본 Git 명령어 정리
- `git status`: 현재 변경 사항 및 Git 상태 확인
- `git log`: 커밋 이력 조회
- `git pull`: 원격 저장소의 변경 사항을 로컬로 가져오기

### 외부 리소스
- [YouTube 강의: Git과 GitHub 초급 튜토리얼](https://www.youtube.com/watch?v=RGOj5yH7evk)
- [YouTube 강의: Git과 GitHub 사용법](https://www.youtube.com/watch?v=tRZGeaHPoaw)
- [GitHub 사용 가이드 (freeCodeCamp)](https://www.freecodecamp.org/news/git-and-github-for-beginners/)




