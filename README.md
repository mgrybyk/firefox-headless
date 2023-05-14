# firefox-headless
Firefox headless with JDK, Maven, NodeJS  
[Docker Hub](https://hub.docker.com/r/atools/firefox-headless)

## Updates

The image updates every week on Wednesday.

## Build

- **JDK_MAVEN_NODE**=`jdk17-nodelts`
- **FIREFOX_VERSION**=`latest`

### Examples

#### Command Line

`docker build --build-arg JDK_MAVEN_NODE=jdk17-nodelts --build-arg FIREFOX_VERSION=latest -f Dockerfile -t firefox .`

#### Jenkins Pipeline

`docker.build('firefox', '--build-arg JDK_MAVEN_NODE=jdk17-nodelts --build-arg FIREFOX_VERSION=latest -f Dockerfile .')`
