# git intro

1. 초기화 `$ git init`
   1. 실제로는 `.git/` 폴더가 생성됨
   2. 버전관리가 시작됨
   3. 리포(repository)라고 부름
2. 서명 설정
   1. `$ git config --global.user.name "name"`
   2. `$ git config --global.user.email "email"`

3. 리포의 상태보기 `$ git status`

4. stage에 올리기 `$ git add` (파일 수정하고 add, index까지..중간단계? 변경사항만 add한다?)

   1. 특정 파일만 올리기 ` $ git add <filename>`
   2. 다 올리기 `$ git add .`

5. snapshot 찍기`$ git commit`(수정한 걸 commit, head로// )

6. 로그 보기 `$ git log`

   

## 집 컴퓨터 세팅

1. git 다운로드 및 설정
2. windows 키 누르고 => git bash 찾아서 실행(집 컴의 홈폴더~)
3. `$ git config --global.user.name "name"`
4. `$ git config --global.user.email "email"`
5. ` $ git clone <url>`



# github

1. 원격 저장소(Remote Repository) 생성
2. 로컬 리포 => 리모트 리포 `$ git remote add origin <url>`
3. 로컬 커밋들을 리모트로 보내기 `$ git push origin master`
4. ` $ git push == $ git push origin mater` 로 단축 명령하기 `git push -u origin master`
5. 다른 컴퓨터에서 리모트 리포 **최초로** 받아오기 ` $ git clone <url>`
6. 이후 리모트 리포 변경사항을 로컬리포에서 반영하기 ` $ git pull `



# TIL 관리 시나리오

1. 멀캠에 온다.
2. ` $ git pull`
3. 열-공
4. 중간 중간 `$ git add . ` & ` $ git commit`
5. 집 가기 전에 `$ git push`
6. 집 도착
7. `$ git pull`
8. 복습 및 자습(`$ git add . ` & `$ git commit`)
9. 마지막으로 `$ git push`
10. 1번으로