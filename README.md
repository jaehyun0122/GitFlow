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

---

# Git flow 실습
#### master branch의 내용을 다른 branch에서 최신을 유지하기 위해 master branch를 merge해준다
#### * git log --decorate --all --graph --oneline
로그를 한줄로 그래프 형식으로 보여준다.

## 1. feature branch
1. git checkout -b feature
2. 작업 후 add & commit

## 2. develop branch
1. develop에서 feature merge / git merge feature
2. git add & commit

## 3. master branch
1. git pull origin master
2. develop merge / git merge develop
3. conflict 있으면 해결
4. git add & commit
5. git push origin master

master에서 수정
