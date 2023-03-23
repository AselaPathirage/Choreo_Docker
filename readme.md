docker build -t helloworld:1.0 .

docker run -d --name helloWorld -p 8080:8080 helloworld:1.0

docker exec -it helloWorld bash

curl localhost:8080

docker tag helloworld:1.0 dmxunlimit/helloworld:1.0

docker push dmxunlimit/helloworld:1.0