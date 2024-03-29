# 명령어

- git reset

  ```
  git reset <branch or commit hash>
  ```

  > reset명령어는 현재 HEAD가 가리키고 있는 브랜치가 바라보고 있는 커밋을 옮기는 명령어

- git cat-file

  ```
  git cat-file -p <object>
  ```

  > Git 레포지토리에 저장되어 있는 데이터를 조회할 때 사용하는 저수준 명령어로서 실무에서는 사실 거의 사용할 일이 없다. 하지만 Git의 내부 구조를 살펴보기 위해 사용할 수 있다. object에는 해시값을 넣으면 된다.

- git diff

  ```
  git diff <commit> <other commit>
  ```

  > diff 명령어는 커밋과 커밋 사이 혹은 현재 작업 중인 디렉터리에서 변경사항을 출력해 주는 명령어

- git add

  ```
  git add <pathspec>
  ```

  > add 명령어는 커밋을 위해 작업 중인 트리에서 현재 내용들을 index에 추가

- git restore

  ```
  git restore <pathspec>
  ```

  > restore 명령어는 작업중인 트리에서 파일을 복원하는 명령어

- git show

  ```
  git show <object>
  ```

  > show 명령어는 blobs, trees 그리고 커밋의 내용을 출력해 주는 명령어

- git log

  ```
  git log
  ```

  > log 명령어는 커밋 로그를 출력해 주는 명령어

- git ls-files

  ```
  git ls-files
  ```

  > ls-files 명령어는 작업중인 트리에서 파일 목록을 출력해 주는 명령어

- git commit --amend

  ```
  git commit --amend
  ```

  > 커밋 메세지를 수정하는 명령어로, 내부적으로 새로운 커밋 메세지를 만들어서 현재브랜치가 새로운 커밋을 바라보게 만드는 것

- git merge

  ```
  git merge <commit | branch name>
  ```

  > 현재 브랜치를 다른 브랜치로 합칠때 사용하는 명령어. 내가 가장 헷갈린 부분은 머지하려는 브랜치로 이동하여 해당 명령어를 실행해야한다는 점. A브랜치로 이동해서 B브랜치를 머지하면 B브랜치가 A브랜치쪽으로 합쳐지는 것.(방향성이 헷갈렸음.)

- git cherry-pick

  ```
  git cherry-pick <commit>
  ```

  > 다른 커밋의 변경사항을 현재 HEAD가 가리키고 있는 브랜치에 적용하는 명령어

- git rebase

  ```
  git rebase <branch>

  ```

  > 새로운 브랜치를 베이스로 하여 브랜치를 하나로 합치는 명령어

- git revert

  ```
  git revert <commit>
  ```

  > revert는 커밋을 되돌리는 명령어이다. 커밋을 삭제해서 되돌리는 것이 아닌, **되돌리는 커밋을 새롭게 추가**하기 때문에 기록이 남는다. 해당 커밋을 단순히 삭제해도 같은 효과가 나지만 그렇게되면 원래 어떤 커밋이 있었고 어떤 이유로 인해 되돌렸다는 기록을 남길수가 없기때문에 reset보다 revert를 사용하는 이유가 되기도 한다. 즉 revert는 특정 커밋을 되돌리고 그 기록을 남기기 위해 사용한다.

- rebase -i ⭐️

  ```
  git rebase -i <commit>
  ```

  > rebase를 사용할 때 -i옵션을 사용하면 여러 커밋들을 수정할 수 있다. 커밋을 삭제하거나, 순서를 변경하거나, 커밋들을 합치거나 특정 커밋을 수정하여 여러 개의 커밋으로 나눌 수 있다. 해당 명령어는 잘 이해하고 직접 사용하는 과정을 통해서 익숙해지면 좋다고 한다. 🙏
