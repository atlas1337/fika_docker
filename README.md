Steps to build on linux:

1. git clone https://github.com/atlas1337/fika_docker fika
2. cd fika
3. docker build --no-cache --label FIKA -t fika .
4. docker run --pull=never -v [server files]:/opt/server --net=host -it --name fika fika
5. docker start fika
6. docker update --restart unless-stopped fika
