# Git
> [Book](https://git-scm.com/book/ko/v2)
## Setting
### init
- 새로운 프로젝트 생성시에 사용한다.
- 해당 프로젝트 폴더로 가서 실행한다.
```shell
$ git init
```
### remote
- github.com 같이 git 저장소를 활용할 경우 remote 설정이 필요하다.
```shell
# remote 연결
$ git remote add origin https://github.com/<본인 계정>/our-project
# 초기 파일들 업로드
$ git push -u origin master
```
### clone
- github.com 등의 저장소에서 프로젝트를 복사해 온다.
```shell
$ git clone https://github.com/<유저이름>/<리포지토리 이름>.git
```
### userName, userEmail
```shell
# 해당 프로젝트
$ git config user.name "hoofacProgram"
$ git config user.email "hoofac.program@gmail.com"
# 시스템 전체
$ git config --global user.name "hoofacProgram"
$ git config --global user.email "hoofac.program@gmail.com"
```

### ignore
- .gitignore 파일에 모듈이나 기타 버전 관리에서 제외할 폴더, 파일 등을 입력한다.
    - .gitignore 자체가 git에 커밋되므로 프로젝트 해당인원 전원에게 해당될 경우만 사용한다.
- .git/info/exclude는 git 업로드 되지 않으므로 개인적인 제외 파일은 여기서 관리한다.
    - ex) .prettierrc
```shell
# 샆(#) 으로 주석을 작성한다.
# 폴더 경로
/node_modules
# 파일 경로
.prettierrc
```

## Log
- log 확인
- 'q' 으로 확인 중단 가능.
```shell
$ git log
```

## Modify commit date 
```shell
$ git commit --amend --no-edit --date "$(date)"
$ git commit --amend --no-edit --date "Sat 24 Dec 2022 23:55:10 KST"
$ git rebase -i HEAD~1
$ GIT_COMMITTER_DATE= git commit --amend --no-edit --date "Sat 24 Dec 2022 23:55:10 KST"
$ GIT_autohor_DATE= git commit --amend --no-edit --date "Sat 24 Dec 2022 23:55:10 KST"
$ $ git rebase --continue
```
