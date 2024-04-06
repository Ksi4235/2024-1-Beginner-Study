git log : commit 기록을 최신순으로 확인  
맨 왼쪽 commit id를 간결하게 확인하려면 --online 붙이면됨  
  
commit id: commit 식별을 위해 사용되는 16진수 수  
  
HEAD 현재 작업중인 branch의 가장 최근 작업을 하면 갱신됨  
commit 되돌리기   
commit --amend :commit을하다가 수정해야할 일이 있을 떄 사용 새로운 commit으로 대체  
git commit --amend -m "커밋 메시지" 커밋 메시지 수정  
git commit --amend --no-edit :메시지 수정없이 commit 수정  
주의: 혼자일때만 사용!!  
  
reset :commit 제거할떄 사용 git reset 옵션 "커맨드 id"==>커맨드 전 기록 다 날림    
1) soft :commit만 취소(파일이 staging area에 돌아옴)  
2) mixed(일반적인 경우) :파일이 working directory로 돌아옴,add부터 수행해야함  
3) hard :커밋완전 취소 작업내용 아예 없어짐  
  
revert : 다른사람이랑 협업할때 주로 사용함  
내용이 추가가 되면 추가된걸 없애는 commit를 만듦  
  
revert --no-edit  이전 커밋으로 작업 디렉토리를 되돌릴 때 사용  
revert	--no-commit  revert한 결과를 stage 상태만 유지하고 commit을 하지 않고싶을 떄 사용  
