# lotte_alttext
2020 멋쟁이사자처럼 해커톤_시각장애인을 위한 롯데 대체텍스트 사이트

# 개발
[강동희](https://github.com/dhk010111)
[고명기](https://github.com/godgi)
[김태형](https://github.com/pletain)
[임도연](https://github.com/dddooo9)
[송요민](https://github.com/alsthd27)

# 시작
1. repository fork

1. 코드 clone

1. 개인 데스크탑에 repository 저장
       
       $ git clone [fork해서 생성된 본인 repository url]
       
1. 로컬에 저장한 프로젝트 폴더에 들어간 후, upstream 설정 
        본인의 repository는 origin, 기존의 repository는 upstream이라고 한다.
        
        $ cd [프로젝트 폴더명]
        
        $ git remote add upstream [fork한 repository url]
       
# 작업
1. branch 생성 및 이동
  가급적 브랜치를 생성하여 새로운 작업을 하고, upstream에서 합쳐진 후에 master에 푸시할 것.
  
    브랜치 생성
    
        $ git branch [brach name]
        
    브랜치 이동    
        
        $ git checkout [branch name]
        
# 작업내용을 upstream에 올리기 
1. 작업한 내용을 유의미하게 commit, add, push
        
        $ git push origin [작업중인 branch name]
        
1. Github의 본인 repository에 들어오면 새로 푸시한 부분을 upstream과 비교하여 merge를 요청할 수 있도록 `Compare & pull request` 라는 버튼이 나타난다.

1. 버튼을 클릭 후 본인 작업한 내용을 요약하여 제목에 적고, 더 상세한 부분은 내용에 작성한다.

1. 우측의 label을 통해 pr을 명확히 한다. 확인을 요청할 경우 반드시 `Review Needed`를 추가하고, 리뷰를 완료한 후 코드 작성자의 확인 및 수정이 필요할 경우 `Revision Required`를 추가한다.

1. 모든 수정과 확인이 완료되면 upstream에 해당 pr의 코드가 merge된다.

1. 해당 pr에 작업한 branch는 merge된 후 `Delete branch`를 통해 삭제하는 것이 좋다.

# 최신 코드 받기
upstream의 master 변경사항을 받을 경우

1. master branch에 위치한 경우
 
        $ git pull upstream master
        
1. 다른 branch에 위치한 경우

        $ git fetch upstream master
        
        $ git merge upstream/master
        
        
