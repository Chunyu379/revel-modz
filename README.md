revel-modz
==========

skeletons & modules for the Revel Framework

this is a work in progress and requires my patch to the `revel new` command
which allows third party skeletons

see: [revel pull #472](https://github.com/robfig/revel/pull/472)

``` Bash
go get github.com/robfig/revel
cd $GOPATH/github.com/robfig/revel
git remote add iassic https://github.com/iassic/revel
git pull iassic
git checkout feature/new-cmd-skeleton-arg
cd revel
go install
```

Installation
--------------

The following instructions will setup a new app with
a skeleton and a grunt file for asset management

``` Bash
go get github.com/iassic/revel-modz
cd $GOPATH/github.com/iassic/revel-modz/modules/grunt
sh install_dependencies.sh
```


Usage
---------------

``` Bash
revel new <APP_NAME> github.com/iassic/revel-modz/skeleton
cd <APP_NAME>
sh npminit.sh
revel run <APP_NAME>
```
