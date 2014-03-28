######################

1) Install docker

2) extract  pumpio_docker.tar.gz

3) go inside folder pump.io

4) configure pump.io.json as per your needs

5) build docker using
docker builder .
    // take care of context, of supervisord and pump.io.json

6)run docker

 docker run -p 22 -p 80:80 -t -v database:/data/db:rw  -v uploads:/var/local/pump.io/uploads:rw <Image Id>
