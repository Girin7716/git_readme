## 이름 설정
![이름설정](https://user-images.githubusercontent.com/52579096/144970720-1b3c17cf-6458-4634-8104-003ee0e766fd.gif)

## 방 입장
![방입장](https://user-images.githubusercontent.com/52579096/144970748-d10531fe-618f-4d32-a714-c962bc40dd7c.gif)

## 채팅
![채팅](https://user-images.githubusercontent.com/52579096/144970761-7a07b639-badf-4f7f-b92e-5713ceab2ea6.gif)

## 이름 변경 & 방 변경
![이름 변경](https://user-images.githubusercontent.com/52579096/144970781-2dd03480-2505-4a4e-a852-2f2db83ead75.gif)

## fast moveShape
![fast moveShape](https://user-images.githubusercontent.com/52579096/144970832-d8d9435e-d232-42b9-a634-1bdfc535d63c.gif)

## slow moveShape
![slow moveShape](https://user-images.githubusercontent.com/52579096/144970856-7c13bd9d-2b92-4f9c-87a6-62b68b0c313b.gif)


## MoveShape
![녹화_2021_12_06_15_54_16_346](https://user-images.githubusercontent.com/52579096/144802667-ae012ee2-2b56-481c-a45f-1c6d27aa5b06.gif)

# Git 사용법

- 참고 영상
  - https://www.youtube.com/watch?v=FXDjmsiv8fI&t=632s

---

## Git 저장소 생성 및 예제 파일 생성
- Git 저장소 생성
  - 컴퓨터에서 원하는 위치에 프로젝트를 진행할 폴더 생성
    - <img src="./git_readme_img/create_git_folder.jpg" width="40%">
  - git init (저장소 만들기)
    - ![git_init](./git_readme_img/git_init.JPG)
  - git config --global user.name "(내 이름)"
    - 내 이름 == 자신의 git hub 이름
    - ![config_name](./git_readme_img/config_name.JPG)
  - git config --global user.email "(내 메일주소)"
    - 내 주소 == 자신의 git hub 이메일 주소
    - ![config_email](./git_readme_img/config_email_moj.JPG)
  - 위 작업 수행 후 숨겨진 파일인 .git 폴더 생성이 됨
    - ![hidden_folder](./git_readme_img/hidden_folder.JPG)
    - .git 폴더는 git 관리 느낌으로 git 저장소 의미

- 예제 파일 생성
  - 저장소 폴더에서 git bash를 실행 한 뒤 리눅스에서 파일 만드는것 처럼 vi (파일이름) 후 내용 적기
  - ex1>cat
    - ![craete_cat](./git_readme_img/create_cat.JPG)
    - <img src="./git_readme_img/contents_cat.JPG" width="40%">
      - 내용 적기 -> esc -> :wq
  - ex2>mouse
    - cat과 똑같이 내용에 name : jerry 적고 저장
  - <img src="./git_readme_img/mouse_cat.JPG" width="50%">
  
---

## 현재 시점 저장하기(add & commit)
- 현재 시점 저장하기 == 타임캡슐에 내용물을 담고 이 내용물이 무엇인지 뜻하는 tag를 달아서 땅바닥에 묻는 작업
- git status
  - 현재 담을게 무엇이 있는지 git 입장에서 살펴보기
  - ![git_status](./git_readme_img/git_status.JPG)
  - 

---

## 이후 새 파일 만들기 & commit 하기
- 예제 파일 만들기
  - dog 파일 만들고 name : snoopy 로 저장
- git status
  - 현재 담을 수 있는것은 dog가 있다는 것을 확인가능.
- git add dog
  - dog 파일을 타임캡슐에 담기
- git commit -m "Add Dog"
  - git status를 입력하면 changes~~ 부분에 타임캡슐에 담긴 내용 확인(dog)
  - git commit -m "Add Dog"
    - 새 캡슐이 묻힌거임

---

## git log (이때까지의 commit 확인)
- git log를 통해 이때까지의 commit 확인해보기

---

## 조금 더 다양한 변화를 주고 commit 해보기
- cat file 삭제
  - rm cat하면 됨
- mouse의 내용물을 name : mickey로 변경
- penguin 파일을 만든 후 name : pororo 작성
- 그 후 git status 확인
  - Untracked files의 penguin == penguin을 담을 수 있다.
  - Changes not staegd for commit에서의 파일들
    - modified -> 수정된 파일
    - deleted -> 삭제된 파일
- 이러한 변화들을 git add -A로 타임캡슐에 담기
- git commit -m "Add Modify Delete"
  -담았으니까 commit하기
- git log로 이때까지의 commit 확인
    - 이때까지 commit한 (First Commit, Add Dog, Add Modify Delte)의 모습을 볼 수 있다.

---

## 현재까지 진행상황
- ![yalco](./git_readme_img/yalco.JPG)

---

## 과거로 돌아가기 - Reset (유튜브 보고 참고하기(06:57~))
- 이전에 묻었던 캡슐(commit)을 파내서 과거의 상태로 돌아가기
- 과감한 방법과 신중한 방법이 있다.
  - 과감한 방법(reset) : 돌아갈 과거 이후 행적은 복원할 여지 없이 삭제
    - 돌아갈 시점을 입력
  - 신중한 방법(revert) : 과거로 돌아가 되 돌아갈 여지를 남김
    - 취소할 시점을 입력
    - git revert (commit 앞의 6자리)

---

## git branch
- 평행우주 넘나들기 == 회사 파일을 건들기에는 무섭고 나는 다른 시도하고 싶을때 사용
- git branch (branch이름)
  - ![branch_my_idea](./git_readme_img/branch_my_idea.JPG)
  - 현 시점에서 두 미래로 분기하겠다라는 뜻
  - 원 branch의 현 상태(내용물)를 그대로 가져옴
- git branch 입력
  - 현재의 branch를 볼 수 있음.
  - ![git_branch](./git_readme_img/git_branch.JPG)
- git checkout (branch 이름)
  - branch 이름에 해당하는 branch로 넘어가기
  - ![git_checkout](./git_readme_img/git_checkout.JPG)
- my-idea branch에서 작업해보기
  - mouse 제거
    - rm mouse
  - dinosaur 생성
    - name : dooly
  - git add -A
  - git commit -m "Add dino"
  - ![do_my_idea](./git_readme_img/do_my_idea.JPG)
- git merge (branch 이름)
  - git checkout master(or main) 입력해서 branch 이동 후
  - git merge my-idea 입력
    - ![git_merge](./git_readme_img/git_merge.JPG)
- git log --graph --all --decorate
  - 시각화된 각 분기에서의 작업 내용을 볼 수 있음
  - ![git_log_all](./git_readme_img/git_log_all.JPG)
