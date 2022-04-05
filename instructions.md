sudo service docker start
docker build --no-cache -t helloworldgodocker .

docker run --name helloworldgodocker -p 8080:80 -tid helloworldgodocker

docker exec -it helloworldgodocker bash

docker rm $(docker ps -aq) -f

docker rmi $(docker images -a -q)