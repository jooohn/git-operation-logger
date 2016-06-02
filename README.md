# git-operation-logger
log git operations

# Installation

```
$ git clone https://github.com/jooohn/git-operation-logger.git ~/.git-operation-logger
$ cd /path/to/any-git-repository
$ ~/.git-operation-logger/bin/install
```

# Usage

```
$ touch first
$ git add first
$ git commit -m 'first commit'
$ git checkout -b develop
$ touch second
$ git add second
$ git commit -m 'second commit'
$ git checkout master
$ git merge develop
```

see logs

```
$ cat ~/.git-operation-log
2016-06-03 00:41:01 /tmp/repos  post-commit master
2016-06-03 00:41:07 /tmp/repos  post-checkout   develop
2016-06-03 00:41:21 /tmp/repos  post-commit develop
2016-06-03 00:41:28 /tmp/repos  post-checkout   master
2016-06-03 00:41:33 /tmp/repos  post-merge  master
```
