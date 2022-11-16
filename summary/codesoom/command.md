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