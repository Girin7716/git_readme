# Git 사용법

- 참고 영상
  - https://www.youtube.com/watch?v=FXDjmsiv8fI&t=632s

---

## Git 저장소 생성 및 예제 파일 생성
- Git 저장소 생성
  - 컴퓨터에서 원하는 위치에 프로젝트를 진행할 폴더 생성
    - <img src="./git_readme_img/create_git_folder.jpg" width="40%">
  - git init (저장소 만들기)
    - ![git_init](./git_readme_img/git_init.jpg)
  - git config --global user.name "(내 이름)"
    - 내 이름 == 자신의 git hub 이름
    - ![config_name](./git_readme_img/config_name.jpg)
  - git config --global user.email "(내 메일주소)"
    - 내 주소 == 자신의 git hub 이메일 주소
    - ![config_email](./git_readme_img/config_email_moj.jpg)
  - 위 작업 수행 후 숨겨진 파일인 .git 폴더 생성이 됨
    - ![hidden_folder](./git_readme_img/hidden_folder.jpg)
    - .git 폴더는 git 관리 느낌으로 git 저장소 의미

- 예제 파일 생성
  - 저장소 폴더에서 git bash를 실행 한 뒤 리눅스에서 파일 만드는것 처럼 vi (파일이름) 후 내용 적기
  - ex1>cat
    - ![craete_cat](./git_readme_img/create_cat.jpg)
    - <img src="./git_readme_img/contents_cat.jpg" width="40%">
      - 내용 적기 -> esc -> :wq
  - ex2>mouse
    - cat과 똑같이 내용에 name : jerry 적고 저장
  - <img src="./git_readme_img/mouse_cat.jpg" width="50%">
  
---

## 현재 시점 저장하기(add & commit)
- 현재 시점 저장하기 == 타임캡슐에 내용물을 담고 이 내용물이 무엇인지 뜻하는 tag를 달아서 땅바닥에 묻는 작업
- git status
  - 현재 담을게 무엇이 있는지 git 입장에서 살펴보기
  - ![git_status](./git_readme_img/git_status.jpg)
  - 

