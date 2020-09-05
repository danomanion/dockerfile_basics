Build and run in the same time 
```
docker build -t <container_name> . && docker run --rm -ti <container_name>
```

Run container and override entrypoint
```
docker run --entrypoint=/bin/bash <container_name>
```

Print environment variables in Linux
```
printenv
```

Building image with defined args 
```
docker build --build-arg <arg_name>=<arg_value> .
```

Running container with ports
```
docker run -ti -p 8888:8888 --rm <image_name>
```

Login to docker hub 
```
docker login
```


