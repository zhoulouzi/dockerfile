wget https://xxx/pinpoint-agent-2.1.0.tar.gz -O pinpoint-agent-2.1.0.tar.gz

docker build -t  zhoulouzi/pinpoint:2.1.0 .

docker build -t  zhoulouzi/pinpoint:2.1.0-init -f ./Dockerfile.init .
