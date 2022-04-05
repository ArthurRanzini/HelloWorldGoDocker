sudo service docker start
docker build --no-cache -t helloworldgodocker .
docker run -p 8080:80 -tid helloworldgodocker
docker exec -it helloworldgodocker bash
docker rmi $(docker images -a -q)