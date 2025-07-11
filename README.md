//모든 파일을 staging area에 추가하기, 수정된 파일만 추가됨
$ git add .

//add한 파일 모두 취소
$ git rm --cached -r .

//특정 파일만 add 취소
$ git rm --cached [파일]

//커밋하기, 수정사유 표시
$ git commit -m "commit message"

//로컬 저장소에서 원격 저장소로 올리기, 브랜치는 웬만하면 main
$ git push origin [브랜치 이름]

※ Tip 8

푸시할 때 항상 main 브랜치에 푸시하도록 설정할 수 있다.

푸시를 할 때 이렇게 명령해보자. (-u는 원격의 main브랜치를 'upstream' 브랜치로 설정하는 옵션이다)

$ git push -u origin main
 

그럼 그 다음부터 푸시할 때는 아래처럼 브랜치 이름을 생략할 수 있다.

//푸시할 때
$ git push

//풀할 때
$ git pull


//저장소 생성 및 연결
$ git init
$ git remote add origin [원격저장소 주소]
$ git branch -m master main

//파일 업로드
$ git pull (또는 git pull origin main)
$ git add .
$ git commit -m "commit message"
$ git push (또는 git push origin main)

//추가적인 명령어
$ git remote -v
$ git remote rm origin
$ git branch
$ git config --global init.defaultBranch [브랜치 이름]
$ git status
$ git rm --cached -r .
$ git push -u origin main
