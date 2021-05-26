# spring-mvc-complete
Spring MVC learnings

## Creating java web application

step 1: Create maven project using mvn commond line utility
```bash
mvn archetype:generate -DgroupId=com.raj.springmvc -DartifactId=spring-mvc-complete 
-DarchetypeArtifactId=maven-archetype-webapp -DinteractiveMode=false
```
Update the `pom.xml` to add servlet dependencies

```
<dependency>
    <groupId>javax.servlet</groupId>
    <artifactId>javax.servlet-api</artifactId>
    <version>3.1.0</version>
    <scope>provided</scope>
</dependency>
```

and tomcat7 plugin
```
<plugin>
   <groupId>org.apache.tomcat.maven</groupId>
   <artifactId>tomcat7-maven-plugin</artifactId>
   <version>2.2</version>
      <configuration>
         <port>9000</port>
         <path>/spring5-webmvc</path>
      </configuration>
</plugin>
```
step 2: Run the web application
