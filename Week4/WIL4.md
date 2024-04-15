##브랜치 관리  
  
####git flow  
branch들은 main branch(자주 사용하는 branch)와 supporting branch 로 나눔  
main branch 사용 후에도 삭제하지 않음  
1)main(master)우리가 아는 main  
2)develop  
  
1.main:영원히 존재하는 첫번쨰 브랜치  
&emsp;병합될때마다 새로운 버전이 탄생  
2.develop:feature 브랜치의 기반이 됨  
  
supporting branch  
feature branch: develop에서 분기하여 작동함 기능 개발후 다시 develop으로 병합됨  
&emsp;&emsp;&emsp;이름은 자유롭지만  대표적인 이름은 안됨  
  
25p그림에서 develop에서 분기됨 commit하면 계속 branch 생성 다 끝난후 병합됨  
  
release branch :develop branch에 있는 것을 배포해야할때 사용  
&emsp;&emsp;&emsp;자잘한 버그를 수정함  
  
hotfix branch:main에서 급작한 버그가 발생했을때 즉각적인 수정 필요한 경우  
&emsp;&emsp;완료후 main과 develop에 다시 병합됨  
   
#### Git hub flow  
배포가 수시로 이루어지는 현 개발 환경에서  git flow는 부적합하다고 판단하여 고안된 내용  
  
release hotfix develop없이 main과 feature만 사용  
검증과정이 없기에 충분히 확인한 후 main으로 merge해야함  
main:main으로 병합전 충분한 test필요  
  
feature: 여러개의 feature branch를 만들어서 동시에 사용  
main에서 분기하여 다시 main으로 병합  
