# CLI 단축키

- ls : 목록확인

- clear : 화면 지우기

- mkdir : make directory, 디렉토리 만들기
    (ex : mkdir 폴더명)
- touch : 파일 생성
  
- rmdir : remove directory
    (ex : rmdir 폴더명)
    
- rm -f : 강제 삭제 (recursive)
- rm -r : 재귀 삭제 (force)


- cd : change directory,  디렉토리 이동 (ex : cd 위치)
- cd .. : 상위 폴더로 이동

- pwd : print working directory, 현재 위치 출력

- bash : CLI 프로그램 

- ctrl + ` : 터미널로 이동
- ctrl + 1 : 반대


# Markdown
- 텍스트 기반의 가벼운 마크업 언어
  
    마크업 : 태그를 이용하여 문서의 구조를 나타내는 것
- 문서의 구조와 내용을 같이 쉽고 빠르게 적고자 탄생
  

- '#' : 제목 표시

- 리스트 : 순서가 있는 리스트와 순서가 없는 리스트(ex : 1.2.3.)
  

- 코드 블럭 : 일반 텍스트와 다르게 코드를 이쁘게 출력 (ex : `code block` , ```code block```)


- 링크 : string은 보여지는 부분, url은 연결할 곳을 나타냄(ex : [string](url))


- 이미지 : 링크와 비슷하지만 이미지를 삽입한다(ex : ![string](img_url))


- 텍스트 강조 : 순서대로 굵게, 기울임, 취소선을 이용해 텍스트를 강조합니다.(ex : **BOLD** , *b* ~~c~~)


- 수평선 : 가로로 긴 수평선을 작성합니다 대개 단락을 구분할 때 사용(ex : ---)

# Git / Github

## README.md
- 프로젝트에 대한 설명 문서
- github 프로젝트에서 가장 먼저 보는 문서
- 일반적으로 소프트웨어와 함께 배포
- 일반적으로 마크다운을 이용해 작성

## Repository
- 특정 디렉토리를 버전 관리하는 저장소
- git init 명령어로 로컬 저장소를 생성
- .git 디렉토리에 버전 관리에 필요한 모든 것이 들어있음.

- 특정 버전으로 남긴다 = commit한다.(3가지 영역을 바탕으로 동작)


## 과정
1. working directory , 작업 영역
2. staging Area, 커밋으로 남기고 싶은 내용
3. repository , 내용들을 모아둔 저장소

- git add : working -> staging
- git commit : staging -> repository
- git status : 현재 상태 확인

### ex
#### case 1 : 기존 로컬 파일 생성후 깃 저장소에 올리는 경우
1. git add README.md
2. git commit -m "EDIT"
3. git remote add origin https://github.com/<본인 계정>/our-project
4. git push -u origin main

#### case 2 : 새로운 저장소를 생성하는 경우

1.  echo "# 파일명" >> README.md
2. git init
3. git add README.md
4. git commit -m "first commit"
5. git branch -M main
6. git remote add origin https://github.com/Jokguking/파일명.git
7. git push -u origin main

※ 저장하고 진행할 것

#### case 3 : add, commit, push 취소

[링크](https://gmlwjd9405.github.io/2018/05/25/git-add-cancle.html)

## EDITMSG 탈출법

- ESC - > :q!

## clone 과 파일 다운로드 차이점
- clone : .git/ 에 변경사항이 저장되어 있음
- 파일 다운로드 : 코드만 가져옴(결과만 필요할 때 사용)






