# GitHub-깃허브 연동하는 방법

1. git init

2. git add .

3. git commit -m "first commit"

4. git branch -M main

5. git remote add origin https: 레포지토리 주소

6. git push -u origin main --> 오류 발생하면 git push -u origin +main 

## (추가)깃허브 연동하는 방법 

이미 리포지토리가 있을 경우 -> git remote remove origin 로 기존 리포지토리 삭제 

1. git remote add origin 리포지토리 주소 

2. git push --set-upstream origin master 실제로 깃허브에 수정한 내역을 반영해주는 것 

error: failed to push some refs to '리포지토리 주소' 오류 발생 이유 

-> local과 github 저장소가 일치하지 않을 때 나타나는 오류. 
 
원칙은 pull -> merge -> push

따라서 git pull origin master로 원격 저장소에 먼저 pull 해줘야한다.

git push -f origin : 강제로 커밋 이력을 덮어씌우는 방법 

작업한 내용이 많다면 -f 옵션으로 푸시하는 것이 좋겠지만, 작업 내용이 많지 않다면 그냥 pull해서 push를 권장 

## 디렉토리 폴더 접근 불가능 오류 

문제 발생 : 깃허브에서 한 디렉토리에 다른 디렉토리를 추가하는 도중 위와 같이 디렉토리에 화살표 표시가 생기고, 디렉토리에 접근이 되지않는 문제가 발생

1. .git 파일 제거
- ls -al로 .git 확인 후
- $ rm -rf .git

2. 스테이지에 존재하는 파일제거
- $ git rm --cached . -rf

3. add - commit - push 진행 




