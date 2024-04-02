## ReadMe.md

static web site

## Build with maven (in GitBash) 
<code>export JAVA_HOME=c:/java/jdk11</code>

<code>cd /c/utils/git/repo/web-static</code>

<code>/c/java/mvn/bin/mvn clean package -f pom.xml</code>

## deploy to localhost
<code>rm -r /c/utils/tomcat/webapps/web-static.war</code>

<code>cp ./target/web-static.war /c/utils/tomcat/webapps</code>

## test
test: http GET to -> http://localhost:8080/web-static/