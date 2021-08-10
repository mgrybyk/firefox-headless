# firefox-headless
Firefox headless with JDK, Maven, NodeJS  
[Docker Hub](https://hub.docker.com/r/atools/firefox-headless)

## Updates

The image updates every week on Wednesday.

## Build

- **JDK_MAVEN_NODE**=`mvn3-jdk11-node14`
- **FIREFOX_VERSION**=`latest`

### Examples

#### Command Line

`docker build --build-arg JDK_MAVEN_NODE=mvn3-jdk11-node14 --build-arg FIREFOX_VERSION=latest -f Dockerfile -t firefox .`

#### Jenkins Pipeline

`docker.build('firefox', '--build-arg JDK_MAVEN_NODE=mvn3-jdk11-node14 --build-arg FIREFOX_VERSION=latest -f Dockerfile .')`
