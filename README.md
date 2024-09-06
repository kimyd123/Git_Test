### 사용설명서 
### 1. 변경도 되는구나
### 2. 짱이네
### 3. 깃허브에서 파일readme 수정 다시
### 4. 새로운것
### 5..dddd

### git log --pretty=oneline
### git show 커밋id 4자리 

### 최근커밋 수정    git commit --amend
### 두 커밋사이 차이점 볼때 git diff 비교하고싶은 커밋 두개
### HEAD는 현재 커밋을 가리키는것
### 커밋변경 git reset --hard eea5         (eea5 << 커밋id)
### --hard  --soft  --mixed
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