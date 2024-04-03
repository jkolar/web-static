## ReadMe.md

static web site

## Build with maven (in GitBash) 
```
export JAVA_HOME=c:/java/jdk11
cd /c/utils/git/repo/web-static
/c/java/mvn/bin/mvn clean package -f pom.xml
```

## deploy to localhost
```
rm -r /c/utils/tomcat/webapps/web-static.war
cp ./target/web-static.war /c/utils/tomcat/webapps
```

## test
test: http GET to -> http://localhost:8080/web-static/