# Spring Framework

```
spring.h2.console.enabled=true
spring.datasource.url=jdbc:h2:file:~/test
spring.datasource.username=sa
spring.datasource.password=
spring.datasource.driver-class-name=org.h2.Driver
```

```
<dependency>
   <groupId>com.h2database</groupId>
   <artifactId>h2</artifactId>
   <scope>runtime</scope>
 </dependency>
 
 <dependency>
	<groupId>org.springframework.boot</groupId>
	<artifactId>spring-boot-starter-data-jpa</artifactId>
</dependency>
```

```
DROP TABLE IF EXISTS user;
 
CREATE TABLE user (
  uid INT AUTO_INCREMENT  PRIMARY KEY,
  email VARCHAR(250) NOT NULL,
  pass VARCHAR(250) NOT NULL
);
 
INSERT INTO user (email, pass) VALUES
 ('mehmet@mail.com', '123456');
```
