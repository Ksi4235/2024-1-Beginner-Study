## Week 1  
vscode에서 github로 파일 올리는 과정  
1.git-scm.com에서 git 설치  
2.git 최초설정  
&emsp;git config --global user.name "깃허브 이름"   
&emsp;git config --global user.email "깃허브 이메일"  
  
3. 디렉토리 생성  
git init 새로운 Git 저장소를 생성할 때 사용하는 Git 명령어  

4.git에 파일 등록하기  
git add : working directory상의 변경 내용을 staging area에 추가하기 위해서 사용하는 Git 명령어   
모든 파일을 한번에 등록 : git add .  
파일 하나씩 등록 : git add 파일명  
올린 파일을 unstage 로 되돌리기  : git rm --cached 파일명
  
5.git의 파일 레포지테리에 저장  
git commit -m "commit message"  
commit message : 내가 저장할 파일에 대한 간단한 설명    

6.git에 파일 올리기  
git push -u origin main 내 브랜치에서 main으로 파일을 push하라  