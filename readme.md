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

## test on local Tomcat
test: http GET to -> http://localhost:8080/web-static/

## deploying it as Azure static web app ...
... is definitelly NOT the same as running it on Tomcat
for example, other then 'default' route has to be specified in 'staticwebapp.config.json'
file in base folder. See 'azure' branch on how is that done
