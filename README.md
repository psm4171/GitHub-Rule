# GitHub-Rule

## VsCode에 깃허브 연동하는 방법 

이미 리포지토리가 있을 경우 -> git remote remove origin 로 기존 리포지토리 삭제 

1. git remote add origin 리포지토리 주소 

2. git push --set-upstream origin master 실제로 깃허브에 수정한 내역을 반영해주는 것 

error: failed to push some refs to '리포지토리 주소' 오류 발생 이유 

-> local과 github 저장소가 일치하지 않을 때 나타나는 오류. 
 
pull -> merge -> push

: git pull origin master로 원격 저장소에 먼저 pull 해줘야한다.
