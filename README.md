# Sample-Logging File for log4j Springboot
## Changes Required

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
    
- Add log4j2 specific dependency
````
        <dependency>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-starter-log4j2</artifactId>
        </dependency>
````

