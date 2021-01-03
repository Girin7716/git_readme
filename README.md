# Git ����

- ���� ����
  - https://www.youtube.com/watch?v=FXDjmsiv8fI&t=632s

---

## Git ����� ���� �� ���� ���� ����
- Git ����� ����
  - ��ǻ�Ϳ��� ���ϴ� ��ġ�� ������Ʈ�� ������ ���� ����
    - <img src="./git_readme_img/create_git_folder.jpg" width="40%">
  - git init (����� �����)
    - ![git_init](./git_readme_img/git_init.jpg)
  - git config --global user.name "(�� �̸�)"
    - �� �̸� == �ڽ��� git hub �̸�
    - ![config_name](./git_readme_img/config_name.jpg)
  - git config --global user.email "(�� �����ּ�)"
    - �� �ּ� == �ڽ��� git hub �̸��� �ּ�
    - ![config_email](./git_readme_img/config_email_moj.jpg)
  - �� �۾� ���� �� ������ ������ .git ���� ������ ��
    - ![hidden_folder](./git_readme_img/hidden_folder.jpg)
    - .git ������ git ���� �������� git ����� �ǹ�

- ���� ���� ����
  - ����� �������� git bash�� ���� �� �� ���������� ���� ����°� ó�� vi (�����̸�) �� ���� ����
  - ex1>cat
    - ![craete_cat](./git_readme_img/create_cat.jpg)
    - <img src="./git_readme_img/contents_cat.jpg" width="40%">
      - ���� ���� -> esc -> :wq
  - ex2>mouse
    - cat�� �Ȱ��� ���뿡 name : jerry ���� ����
  - <img src="./git_readme_img/mouse_cat.jpg" width="50%">
  
---

## ���� ���� �����ϱ�(add & commit)
- ���� ���� �����ϱ� == Ÿ��ĸ���� ���빰�� ��� �� ���빰�� �������� ���ϴ� tag�� �޾Ƽ� ���ٴڿ� ���� �۾�
- git status
  - ���� ������ ������ �ִ��� git ���忡�� ���캸��
  - ![git_status](./git_readme_img/git_status.jpg)
  - Untracked file(���� �۾�) == ���� ����� ���� ���ϵ�
    - ��Ȯ���� �� ���ϵ��� ��������ٴ� ��ǵ�
    - ������ git_readme_img�� �����ϸ� ��(����� �̹���)
- git add -A
  - �̰��� ��� ���� git�� Ÿ��ĸ���� �ְڴ�.
  - ![git_add](./git_readme_img/git_add.jpg)
  - �� �� git status �Է��ϸ�
    - ![status_after_add](./git_readme_img/status_after_add.jpg)
    - Changes to be comitted == ���� �͵��� �ǹ�
- git commit -m "����"
  - Ÿ��ĸ���� ���� �۾� + Ÿ��ĸ�� ���� ����
  - ![git_commit_first](./git_readme_img/git_commit_first.jpg)
  - ���� git status�� �ϸ� ������ ���ٰ� ����.

## ���� �� ���� ����� & commit �ϱ�
- ���� ���� �����
  - dog ���� ����� name : snoopy �� ����
    - <img src="./git_readme_img/create_dog.jpg" width="50%">
- git status
  - <img src="./git_readme_img/untracked_dog.jpg" width="50%">
  - ���� ���� �� �ִ°��� dog�� �ִ�.
- git add dog
  - dog ������ Ÿ��ĸ���� ���
  - ![git_add_dog](./git_readme_img/git_add_dog.jpg)
- git commit -m "Add Dog"
  - git status�� �Է��ϸ� changes~~ �κп� Ÿ��ĸ���� ��� ���� Ȯ��(dog)
    - <img src="./git_readme_img/status_after_add_dog.jpg" width="100%">
  - git commit -m "Add Dog"
    - ![git_commit_dog](./git_readme_img/git_commit_dog.jpg)
    - �� ĸ���� ��������

## git log (�̶������� commit Ȯ��)
- git log
  - ![git_log](./git_readme_img/git_log.jpg)

## ���� �� �پ��� ��ȭ�� �ְ� commit �غ���
- cat file ����
  - ![remove_cat](./git_readme_img/remove_cat.jpg)
- mouse�� ���빰�� name : mickey�� ����
- penguin ������ ���� �� name : pororo �ۼ�
  - ![create_penguin](./git_readme_img/create_penguin.jpg) 
- �� �� git status Ȯ��
  - ![after_git_status2](./git_readme_img/after_git_status2.jpg)
    - Untracked files�� penguin == penguin�� ���� �� �ִ�.
    - Changes not staegd for commit������ ���ϵ�
      - modified -> ������ ����
      - deleted -> ������ ����