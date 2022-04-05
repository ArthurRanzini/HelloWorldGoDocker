sudo service docker start
docker build -t helloworldgodocker .
docker run -p 8080:80 -tid helloworldgodocker