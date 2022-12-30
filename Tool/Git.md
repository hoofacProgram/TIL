# Git
> [Book](https://git-scm.com/book/ko/v2)
## Setting
### userName, userEmail
```
$ git config --global user.name "hoofacProgram"
$ git config --global user.email "hoofac.program@gmail.com"
```

### ignore
- .gitignore 파일에 모듈이나 기타 버전 관리에서 제외할 폴더, 파일 등을 입력한다.
    - .gitignore 자체가 git에 커밋되므로 프로젝트 해당인원 전원에게 해당될 경우만 사용한다.
- .git/info/exclude는 git 업로드 되지 않으므로 개인적인 제외 파일은 여기서 관리한다.
    - ex) .prettierrc


## Log
- log 확인
- 'q' 으로 확인 중단 가능.
```
$ git log
```

## Modify commit date 
```
$ git commit --amend --no-edit --date "$(date)"
$ git commit --amend --no-edit --date "Sat 24 Dec 2022 23:55:10 KST"
$ git rebase -i HEAD~1
$ GIT_COMMITTER_DATE= git commit --amend --no-edit --date "Sat 24 Dec 2022 23:55:10 KST"
$ GIT_autohor_DATE= git commit --amend --no-edit --date "Sat 24 Dec 2022 23:55:10 KST"
$ $ git rebase --continue
```
