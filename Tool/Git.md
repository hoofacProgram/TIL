# Git
> [Book](https://git-scm.com/book/ko/v2)
## Setting
- userName, userEmail
```
$ git config --global user.name "hoofacProgram"
$ git config --global user.email "hoofac.program@gmail.com"
```

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
