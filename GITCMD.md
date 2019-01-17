# 깃 커맨드
### 도움말
command | task
--- | ---
git | 도움말 개요 보기
git <커맨드> --help | 특정 커맨드에 대한 도움말 보기
### 생성
command | task
--- | ---
**git init** | 새로운 로컬 레포지토리 생성
git clone username@host:/path/to/repository | 원격 레포지토리를 로컬로 복사
### 인증
command | task
--- | ---
git config --global user.name "<유저명>" | 커밋에 쓸 유저명 설정
git config --global user.email <이메일> | 커밋에 쓸 이메일 설정
git config credential.helper store | 인증 정보 저장 (저장 직후 푸쉬할 때 한 번 더 기입 필요)
### 로컬
command | task
--- | ---
**git status** | 스테이지 보기
**git add <파일명>** | 스테이지에 파일 등록
git add -A | 스테이지에 모든 파일 등록
**git commit -m "<메세지>"** | 커밋 메세지를 가지고 커밋하기
git diff | 머지 컨플릭트(merge conflict) 보기
git log | 커밋 로그 보기
### 원격
command | task
--- | ---
git remote -v | 현재 연결된 모든 리모트 레포지토리 보기
**git remote add origin <서버>** | 오리진이란 이름으로 원격 레포지토리에 연결
**git push -u origin master** | 커밋을 원격 레포지토리에 푸쉬 (트래킹 레퍼런스)
git pull | 원격 레포지토리를 로컬로 다운받아서 머지
### 브랜치
command | task
--- | ---
git branch -a | 모든 로컬과 원격 브랜치 보기
git branch <브랜치이름> | 브랜치 생성
git checkout <브랜치이름> | 브랜치로 이동
git branch -d <브랜치이름> | 브랜치 삭제
git push origin <브랜치이름> | 특정 원격 브랜치로 푸쉬
git push origin :<브랜치이름> | 원격 브랜치 삭제
git merge <브랜치이름> | 한 브랜치를 현재 브랜치로 머지
