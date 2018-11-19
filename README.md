# Maven Docker Image with Aliyun Mirror

This image is built from official Maven Docker image with [Aliyun Mirror](http://maven.aliyun.com/).

### Run a single Maven command

For many simple projects, you may find it inconvenient to write a complete Dockerfile. In such cases, you can run a Maven project by using the Maven Docker image directly, passing a Maven command to docker run:

```
docker run -it --rm --name my-maven-project -v "$(pwd)":/usr/src/mymaven -w /usr/src/mymaven registry.cn-hangzhou.aliyuncs.com/acs/maven mvn clean install
```

### More usages

Please refer the documents for [official Maven image](https://github.com/carlossg/docker-maven).

Contributors
-------------------
* Li Yi (denverdino@gmail.com)

