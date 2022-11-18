# my-spring-boot-domo
Added

demo.cljc

jupyter_helpers.cljc

Build the jar package for Java calls

1. jupyter notebook init.ipynb file

Execute :

`%%bash
lein uberjar
`

or

In the idea

Click Tasks => uberjar

After execution:

ppdsp-0.1.0-SNAPSHOT-standalone.jar

2. Import ppdsp-0.1.0-SNAPSHOT-standalone.jar into the maven repository

 ```
 mvn install:install-file -Dfile="ppdsp-0.1.0-SNAPSHOT-standalone.jar" -DgroupId=com.ppdsp -DartifactId=noise.addition.variations -Dversion=0.1.0-SNAPSHOT -Dpackaging=jar

 ```
 
 3.Building Java WEB Services
 
 and produce the jar package (demo-0.0.1-SNAPSHOT.jar)
```
   mvn  -DskipTests=true package
   ```
   or

   idea build
   Lifecycle =>package
   
4. Start web service

 ```
       Java -jar  demo-0.0.1-SNAPSHOT.jar
        ```
        
 Run idea
