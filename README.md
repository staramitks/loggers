# loggers
Sample-Logging File for log4j
# For Springboot projects two changes are required in pom.xml
## 
 - Remove default logging provided by springboot
 ````
    <dependency>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-starter-web</artifactId>
			<exclusions>
				<exclusion>
					<groupId>org.springframework.boot</groupId>
					<artifactId>spring-boot-starter-logging</artifactId>
				</exclusion>
			</exclusions>
    </dependency>
    
    ````
    
##
  - Add a dedicated log4j2 dependency
````
        <dependency>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-starter-log4j2</artifactId>
        </dependency>
````

