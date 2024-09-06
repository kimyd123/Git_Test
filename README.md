

### HEAD는 현재 커밋을 가리키는것

### git log
커밋 히스토리를 출력

### git log --pretty=oneline
--pretty 옵션을 사용하면 커밋 히스토리를 다양한 방식으로 출력할 수 있습니다. --pretty 옵션에 oneline이라는 값을 주면 커밋 하나당 한 줄씩 출력

### git show [커밋 아이디]
특정 커밋에서 어떤 변경사항이 있었는지 확인

### git commit --amend 
최신 커밋을 다시 수정해서 새로운 커밋으로 만듦

### git config alias.[별명] [커맨드]
길이가 긴 커맨드에 별명을 붙여서 이후로 별명으로 해당 커맨드를 실행할 수 있도록 설정

### git diff [커밋 A의 아이디] [커밋 B의 아이디]
두 커밋 간의 차이 비교

### git reset [옵션] [커밋 아이디]  
### 옵션 : --hard  --soft  --mixed
옵션에 따라 하는 작업이 달라짐(옵션을 생략하면 --mixed 옵션이 적용됨)

(1) HEAD가 특정 커밋을 가리키도록 이동시킴(--soft는 여기까지 수행)

(2) staging area도 특정 커밋처럼 리셋(--mixed는 여기까지 수행)

(3) working directory도 특정 커밋처럼 리셋(--hard는 여기까지 수행)


staging area와 HEAD의 개념을 반영해서 정리하자면 git reset 후 복구를 위해선

-- soft :
git commit

--mixed :
git add .
git commit

--hard : 
git pull

### git reset --hard HEAD^   
현재 HEAD가 가리키고 있는 커밋의 바로 이전 커밋
### git reset --hard HEAD~2
현재 HEAD가 가리키는 커밋보다 2단계 전에 있는 커밋

## git tag [태그 이름] [커밋 아이디]
특정 커밋에 태그를 붙임


-----------------------
### 브랜치
 master branch 는 기본 브랜치