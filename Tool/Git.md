# Git
> [Book](https://git-scm.com/book/ko/v2)
## Setting
### init
- 새로운 프로젝트 생성시에 사용한다.
- 해당 프로젝트 폴더로 가서 실행한다.
```shell
$ git init
```

### userName, userEmail
```shell
# 해당 프로젝트
$ git config user.name "github name"
$ git config user.email "github id email"
# 시스템 전체
$ git config --global user.name "github name"
$ git config --global user.email "github id email"
```

### remote
- github.com 같이 git 저장소를 활용할 경우 remote 설정이 필요하다.
```shell
# remote 연결
$ git remote add origin git@github.com:{github name}/KIS_stock.git
# 초기 파일들 업로드
$ git push -u origin master
```

### clone
- github.com 등의 저장소에서 프로젝트를 복사해 온다.
```shell
$ git clone https://github.com/<유저이름>/<리포지토리 이름>.git
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

### private repository
- ssh와 ssh-keygen을 이용해서 접속 환경을 설정한다.
- ssh-keygen 생성하고 .ssh > id_rsa.pub 내용 복사.
- github 접속, 해당 ID의 settings > SSH and GPG keys > SSH keys의 New SSH key 누르고 id_rsa.pub 내용 입력해서 keys 생성.
```shell
# ssh-keyhen 생성
$ ssh-keygen -t rsa -C "github id email"
```

- 이후에는 기본 셋팅 시작
```shell
$ git init
$ git config user.name "github name"
$ git config user.email "github id email"
$ git remote add origin git@github.com:{github name}/KIS_stock.git
$ git add .gitignore    # add용 파일은 미리 생성해놔야 한다.
$ git commit -m 'create gitignore'
$ git branch -M main
$ git push -u origin main
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
