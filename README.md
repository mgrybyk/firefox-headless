# firefox-headless
Firefox headless with JDK, Maven, NodeJS  
[Docker Hub](https://hub.docker.com/r/atools/firefox-headless)

## Build

You may build image with desired versions of JDK, Maven and NodeJS:
- **JDK_MAVEN_NODE**=`mvn3-jdk8-node12` see available versions - [jdk-maven-node](https://hub.docker.com/r/atools/jdk-maven-node/tags)
- **FIREFOX_VERSION**=`latest` see available version - [firefox releases](https://ftp.mozilla.org/pub/firefox/releases/)

### Examples

#### Command Line

`docker build --build-arg JDK_MAVEN_NODE=mvn3-jdk8-node12 --build-arg FIREFOX_VERSION=latest -f Dockerfile -t firefox .`

#### Jenkins Pipeline

`docker.build('firefox', '--build-arg JDK_MAVEN_NODE=mvn3-jdk8-node-12 --build-arg FIREFOX_VERSION=latest -f Dockerfile .')`
