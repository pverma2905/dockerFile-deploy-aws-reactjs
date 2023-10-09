1)docker build -t image_react:v1 .
2)docker run -it -d -p 3001:3000 --name rc1 image_react:v1
3)docker stop rc1
4)docker commit rc1 pranavv481/image_react:tagname
5)docker push pranavv481/image_react:tagname

deploy
6)docker pull pranavv481/image_react:tagname
7)docker run -it -d -p 3001:3000 --name rc1 pranavv481/image_react:tagname

