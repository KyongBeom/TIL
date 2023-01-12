**2023-01-12/ markdown all in one 설치**

### GUI(Graphic User Interface)
그래픽을 통해 사용자와 컴퓨터가 상호작용/일상 폴더나 바탕화면

### CLI(Command Line Interface)
명령어를 통해 사용자와 컴퓨터가 상호작용/cmd

#### CLI를 사용하는 이유
 > GUI는 CIL보다 사용하기 쉽지만 단계가 많고 컴퓨터 사양을 더 소모
  수많은 서버/개발 시스템이 CLI를 통한 조작 환경을 제공

### 절대 경로
> - 루트 디렉토리부터 목적 지점까지 거치는 모든 경로를 전부 작성한 것
> - 윈도우 바탕 화면의 절대 경로 C:/Users/ssafy/desktop

### 상대 경로
 >- 현재 작업하고 있는 디렉토리를 기준으로 계산된 상대적 위치를 작성한 것
 >- 현재 작업하고 있는 디렉토리가 C:/Users 일 때
 >-  윈도우 바탕 화면으로의 상대 경로는 ssafy/desktop
 >- ./: 현재 작업하고 있는 폴더 ../: 현재 작업하고 있는 폴더의 부모 폴더
  
# 마크 다운(mark down)
 **텍스트 기반의 가벼운 마크업(markup)언어**
 ```text  
  마크업 : 태그를 이용하여 문서의 구조를 나타내는 것
  문서의 구조와 내용을 같이 쉽고 빠르게 적고자 탄생

        #(헤딩)               : 문서의 제목이나 소제목으로 사용
        1.2.3.(리스트)        : 순서가 있는 리스트와 순서가 없는 리스트
   ``` .. ```(코드 블럭)      : 일반 텍스트와 다르게 코드를 이쁘게 출시
      [..](url)(링크)         : ..은 보여지는 부분, url은 연결한 곳
 ![..](img_url)(이미지)       : 이미지 등장
텍스트 강조(** **,* *,~~ ~~)  : 텍스트 강조
             ---(수평선)      : 가로로 긴 수평선 작성

   위 내용은 https://www.markdownguide.org/cheat-sheet/ 에 있습니다.
```
# GIT - 버전 관리

- 버전 : 컴퓨터 소프트웨어의 특정상태
- 관리: 어떤 일의 사무, 시설이나 물건의 유지/개량
- 프로그램: 컴퓨터에서 실행될 때 특정 작업을 수행하는 일련의 명령어들의 모음

>코드의 히스토리(버전)을 관리하는 도구
>- 개발되어온 과정 파악 가능
>- 이전 버전과의 변경 사항 비교 및 분석

## Repository - 특정 디렉토리를 버전 관리하는 저장소
 - git init 명령어로 로컬 저장소를 생성
 - .git 디렉토리에 버전 관리에 필요한 모든 것이 들어있음
 - 특정 버전으로 남긴다 = "커밋(commit)한다"

### 순서  
- working directory -> 작업 영역
- Staging Area -> commit으로 남기고 싶은 내용
- repository -> commit 중에서 남기고 싶은 내용만
  ![git image](https://miro.medium.com/max/640/1*zpvd5fjZAFGsVAEsvMGKxA.webp)
 ### git 명령어
 - git add : working -> staging
 - git commit : staging -> repository ex)git commit-m "add README.md" /- commit 한 제목
 - git remote add origin https: //~~~~ : 뒤 url 을 origin 으로 부르겠다. 
 - git remote -v : github 에 연결 되었는지 확인
 - git push -u origin main: 인터넷에 올리기
 - git log : 기록 확인
 - git branch -M main : master 였던 걸 main 으로 변경
 - git status : 현재 상태 확인 
 * VIM 탈출법 : ESC -> : > q > !
 * Enter 탈출법 : q
 > git clone 과 download 의 차이 : .git의 유무 즉, 변경 이력을 알 수 없음.

# 명령어/bash에서 사용
 - ls: 목록 확인
 - clear : 화면 지우기
 - mkdir : make directory, 디렉토리 만들기
   -  ex) mkdir (폴더명)
 - cd : change directory, 디렉토리 이동
   -  ex) cd (위치)
 -  cd .. : 상위 폴더로 이동
 - pwd : print working directory, 현재 위치 파악
 - find -name (폴더명) : 디렉토리 찾기
 - rmdir : remove directory
   -  ex) redir (폴더명)
      -   rm -r : 삭제시 하위 경로 모든 파일과 폴더 삭제
       -   rm -f : 안 물어보고 삭제 ***조심해서 사용
 - touch : 파일을 생성
 - start, open : 폴더/파일을 여는 명령어

사용 편의
- tap : 앞글자에서 가장 가깝거나 비슷한 글자 바로 탄생
  - ex) de + tap -> desktop