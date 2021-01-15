


docker build -t wenhsiaoyi/sencha6:6.5.3 -t wenhsiaoyi/sencha6:6.5.3 .


## build image
docker build -t wenhsiaoyi/sencha6:6.5.3
docker login
docker push wenhsiaoyi/sencha6:6.5.3




docker run --rm -it wenhsiaoyi/sencha6:6.5.3


alias sencha65='docker run --env JAVA_OPTS="-Xms64M -Xmx4G" -it  -p 1841:1841 -p 1842:1842 --rm -v $PWD:`pwd` -w `pwd` --name sencha653 wenhsiaoyi/sencha6:6.5.3 sencha'




## git log 查詢 commit 的檢查碼


# 忽略 在目錄下新增一個名為 .gitignore 的檔案
touch .gitignore
nano .gitignore

加入路徑與檔名

# 清除cache
git rm --cached

# 清除忽略的檔案
git clean -fX


透過 git checkout -- <file> 來還原檔案的內容

使用 git rm <file> 來告知 git，哪些是我們將要刪除的檔案

使用 git add -u 加入所有被更動的檔案（包含 modified 及 deleted）

使用 git mv <file> <new_name> 來重新命名檔案



###加入該次commit的檢查碼
$ git tag -a v6.5.3.6 0b8805023f9

$ git tag




$ git push origin bionic
$ git push origin --tags


git revert HEAD --no-edit

git reset HEAD

git add filename

git commit  -m ""


# 檔案異動
git add filename
git commit -m "up"
git push




Method 1. Use /etc/*-release file to display Linux distro version
To find out what version of Linux (distro) you are running, enter the following cat command at the shell prompt:
$ cat /etc/*-release




docker pull maven:3.6-openjdk-8


