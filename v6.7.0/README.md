# sencha6

## build image
docker build -t wenhsiaoyi/sencha6:6.7.0 .
docker login
docker push wenhsiaoyi/sencha6:6.7.0




alias sencha67='docker run --env JAVA_OPTS="-Xms64M -Xmx4G" -it  -p 1841:1841 -p 1842:1842 --rm -v $PWD:`pwd` -w `pwd` --name sencha670 wenhsiaoyi/sencha6:6.7.0 sencha'


第一次
docker run --env JAVA_OPTS="-Xms64M -Xmx4G" -it  -p 1841:1841 -p 1842:1842 --rm -v $PWD:`pwd` -w `pwd` --name sencha670 wenhsiaoyi/sencha6:6.7.0 sencha
 


git log 查詢 commit 的檢查碼

加入該次commit的檢查碼
$ git tag -a v6.7.0 9fceb02

$ git tag




$ git push origin v6.7.0
$ git push origin --tags


