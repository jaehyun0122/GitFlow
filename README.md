# Git Flow

git을 생성하면 기본적으로 master브렌치에서 작업을 하게 된다.

feature브렌치에서 특정 작업을 수행한다.

feature브렌치에서 작업한 내용을 develop브렌치로 merge



release브렌치 : master로 push 전 release브렌치에서 버그와 같은 것을 수정

=> 테스트까지 맡이면 master브렌치로 merge

=> 계속 작업해야되기 때문에 develop브렌치로도 merge





git tag -a _ -m "comment" master



push & pull

자주하면 좋다.

develop에서 작업을 하다가 feature를 생성하기전에 pull을 받아 변경사항을 확인한다.

feature에서 작업한 내용을 develop



- git branch (로컬 브랜치 목록 조회) 
- git branch -r (원격 브랜치 목록 조회) 
- git branch -a (모든 브랜치 목록 조회)

출처: <https://ifuwanna.tistory.com/283> [IfUwanna IT]

 1. feature branch // develop branch에서 수정
 2. develop branch