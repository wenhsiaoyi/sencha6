# sencha7

## build image
docker build -t wenhsiaoyi/sencha6:7.3.0jammy .
docker login
docker push wenhsiaoyi/sencha6:7.3.0jammy




alias sencha7='docker run --env JAVA_OPTS="-Xms64M -Xmx4G" -it  -p 1841:1841 -p 1842:1842 --rm -v $PWD:`pwd` -w `pwd` --name sencha730 wenhsiaoyi/sencha6:7.3.0jammy sencha'


第一次
docker run --env JAVA_OPTS="-Xms64M -Xmx4G" -it  -p 1841:1841 -p 1842:1842 --rm -v $PWD:`pwd` -w `pwd` --name sencha730jammy wenhsiaoyi/sencha6:7.3.0jammy sencha
 


git log 查詢 commit 的檢查碼

加入該次commit的檢查碼
$ git tag -a v7.3.0jammy c626b7404cd27dbfec01417a11c40ca1421c4cfd

$ git tag




$ git push origin v7.3.0jammy
$ git push origin --tags


