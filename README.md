Repository - 특정 디렉토리를 버전 관리하는 저장소
 -git init 명령어로 로컬 저장소를 생성
 -.git 디렉토리에 버전 관리에 필요한 모든 것이 들어있음
 -특정 버전으로 남긴다 = "커밋(commit)한다"

 working directory -> 작업 영역
 Staging Area -> commit으로 남기고 싶은 내용
 repository -> commit 중에서 남기고 싶은 내용만
 
 git 명령어
 git add : working -> staging
 git commit : staging -> repository ex)git commit-m "add README.md" /commit 한 제목
 git remote add origin https://~~~~ : 뒤 url 을 origin 으로 부르겠다. 
 git remote -v : github 에 연결 되었는지 확인
 git push -u origin main: 인터넷에 올리기
 git log : 기록 확인
 git branch -M main : master 였던 걸 main 으로 변경
 git status : 현재 상태 확인 
 *VIM 탈출법 : ESC -> : > q > !
 *Enter 탈출법 : q
 git clone 과 download 의 차이 : .git의 유무 즉, 변경 이력을 알 수 없음.