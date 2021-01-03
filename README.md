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
  - 

---

## ���� �� ���� ����� & commit �ϱ�
- ���� ���� �����
  - dog ���� ����� name : snoopy �� ����
- git status
  - ���� ���� �� �ִ°��� dog�� �ִٴ� ���� Ȯ�ΰ���.
- git add dog
  - dog ������ Ÿ��ĸ���� ���
- git commit -m "Add Dog"
  - git status�� �Է��ϸ� changes~~ �κп� Ÿ��ĸ���� ��� ���� Ȯ��(dog)
  - git commit -m "Add Dog"
    - �� ĸ���� ��������

---

## git log (�̶������� commit Ȯ��)
- git log�� ���� �̶������� commit Ȯ���غ���

---

## ���� �� �پ��� ��ȭ�� �ְ� commit �غ���
- cat file ����
  - rm cat�ϸ� ��
- mouse�� ���빰�� name : mickey�� ����
- penguin ������ ���� �� name : pororo �ۼ�
- �� �� git status Ȯ��
  - Untracked files�� penguin == penguin�� ���� �� �ִ�.
  - Changes not staegd for commit������ ���ϵ�
    - modified -> ������ ����
    - deleted -> ������ ����
- �̷��� ��ȭ���� git add -A�� Ÿ��ĸ���� ���
- git commit -m "Add Modify Delete"
  -������ϱ� commit�ϱ�
- git log�� �̶������� commit Ȯ��
    - �̶����� commit�� (First Commit, Add Dog, Add Modify Delte)�� ����� �� �� �ִ�.

---

## ������� �����Ȳ
- ![yalco](./git_readme_img/yalco.jpg)

---

## ���ŷ� ���ư��� - Reset (��Ʃ�� ���� �����ϱ�(06:57~))
- ������ ������ ĸ��(commit)�� �ĳ��� ������ ���·� ���ư���
- ������ ����� ������ ����� �ִ�.
  - ������ ���(reset) : ���ư� ���� ���� ������ ������ ���� ���� ����
    - ���ư� ������ �Է�
  - ������ ���(revert) : ���ŷ� ���ư� �� ���ư� ������ ����
    - ����� ������ �Է�
    - git revert (commit ���� 6�ڸ�)
