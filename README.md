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
  - Untracked file(빨간 글씨) == 아직 담기지 않은 파일들
    - 정확히는 이 파일들이 만들어졌다는 사실들
    - 앞으로 git_readme_img는 무시하면 됨(리드미 이미지)
- git add -A
  - 이곳의 모든 것을 git의 타임캡슐에 넣겠다.
  - ![git_add](./git_readme_img/git_add.jpg)
  - 그 후 git status 입력하면
    - ![status_after_add](./git_readme_img/status_after_add.jpg)
    - Changes to be comitted == 묻을 것들을 의미
- git commit -m "내용"
  - 타임캡슐을 묻는 작업 + 타임캡슐 내용 적기
  - ![git_commit_first](./git_readme_img/git_commit_first.jpg)
  - 이후 git status를 하면 묻을게 없다고 나옴.

## 이후 새 파일 만들기 & commit 하기
- 예제 파일 만들기
  - dog 파일 만들고 name : snoopy 로 저장
    - <img src="./git_readme_img/create_dog.jpg" width="50%">
- git status
  - <img src="./git_readme_img/untracked_dog.jpg" width="50%">
  - 현재 담을 수 있는것은 dog가 있다.
- git add dog
  - dog 파일을 타임캡슐에 담기
  - ![git_add_dog](./git_readme_img/git_add_dog.jpg)
- git commit -m "Add Dog"
  - git status를 입력하면 changes~~ 부분에 타임캡슐에 담긴 내용 확인(dog)
    - <img src="./git_readme_img/status_after_add_dog.jpg" width="100%">
  - git commit -m "Add Dog"
    - ![git_commit_dog](./git_readme_img/git_commit_dog.jpg)
    - 새 캡슐이 묻힌거임

## git log (이때까지의 commit 확인)
- git log
  - ![git_log](./git_readme_img/git_log.jpg)

## 조금 더 다양한 변화를 주고 commit 해보기
- cat file 삭제
  - ![remove_cat](./git_readme_img/remove_cat.jpg)
- mouse의 내용물을 name : mickey로 변경
- penguin 파일을 만든 후 name : pororo 작성
  - ![create_penguin](./git_readme_img/create_penguin.jpg) 
- 그 후 git status 확인
  - ![after_git_status2](./git_readme_img/after_git_status2.jpg)
    - Untracked files의 penguin == penguin을 담을 수 있다.
    - Changes not staegd for commit에서의 파일들
      - modified -> 수정된 파일
      - deleted -> 삭제된 파일