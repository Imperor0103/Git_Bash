Practice Git Bash

user.name은 GitHub activity에 남는 아이디를 기준으로 작성한다(0103 붙인다)

copy: ctrl shift insert
paste: ctrl shift insert

git add 폴더경로
git commit -m "커밋 메시지"

git add MyFolder
git commit -m "MyFolder 안의 모든 변경 사항 커밋"

git add .
git commit -m "모든 변경 사항 커밋"

상태 확인
git status

아직 git add 하지 않은 변경 사항 되돌리기
git restore 파일명

git add 한 파일을 unstaged 상태로 되돌리기
git restore --staged 파일명

commit한 변경 사항 되돌리기(이전 commit으로 되돌리고 싶을 때)
마지막 커밋 하나만 취소 (단, 아직 push 전이라면 안전)
git reset --soft HEAD~1  # 커밋만 취소, 변경 내용은 남김
git reset --hard HEAD~1  # 커밋도, 변경 내용도 모두 삭제

특정 파일만 이전 커밋으로 복구
git checkout HEAD -- 파일명
또는
git restore --source=HEAD 파일명

현재 디렉터리(경로) 확인하기
pwd

디렉터리 안 파일들 목록 보기
ls

특정 파일의 전체 경로 보기
realpath 파일이름

git 프로젝트 루트 경로 보기
git rev-parse --show-toplevel


