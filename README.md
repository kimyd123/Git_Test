

### HEAD는 현재 커밋을 가리키는것


### git log --pretty=oneline
커밋 한줄로 편하게 보는것

### git show [커밋 아이디]
커밋 상세수정내용 보기

### git commit --amend
최근 커밋 수정 

### git diff [커밋 아이디] [커밋 아이디]
두 커밋사이 차이점 볼때  비교하고싶은 커밋 두개

### git reset [옵션] [커밋 아이디]  
### 옵션 : --hard  --soft  --mixed
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
git show [태그 이름]
