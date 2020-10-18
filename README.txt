<Git & GitHub>
1. 로컬 저장소
- git init
: .git폴더 만들기(버전들의 정보, 원격저장소 주소 등)

- git config --global user.email "2chaekyeong@gmail.com"
  git config --global user.name "2chaekyeong"
: github계정 입력

- git add hi.txt
: hi.txt파일을 올릴 것이다.

- git commit -m "메세지 입력"
: 설명을 추가해준다.

+ 파일을 수정했다면 다시

- git add hi.txt

- git commit -m "수정된 메세지 입력"

+ 되돌아 갈려면

- git log
: 로그가 나온다.

- git checkout [커밋 아이디 복사]

- git checkout -
: 최신 커밋으로 돌아가기
 
2. 로컬 저장소 -> 원격 저장소
- github에 접속하여 원격 저장소(new repository)생성
- 원격 저장소 주소 복사하기

- git remote add origin [주소 복사]
: remote add origin(원격 저장소 주소 알려주기)

- git push origin master
: push명령어로 원격저장소에 올리기

3. 원격 저장소 -> 로컬 저장소
- git clone [원격 저장소 주소] . (여기서 띄어쓰고 .을 해주어야 새로운 폴더가 안 생긴다.)

+ 파일을 수정한 후 다시
- git add README.txt
- git commit -m "수정된 메세지"
- git push origin master

4. 원격 저장소에 있는것이 수정된것이 있다면?
- git pull origin master
: pull(원격 저장소에 수정된 것이 있다면 받아오겠다.)
