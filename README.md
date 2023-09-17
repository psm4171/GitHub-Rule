# GitHub-깃허브 연동하는 방법

git init
git add .
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/psm4171/NHNlog.git
git push -u origin main --> 오류 발생하면 git push -u origin +main 

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




