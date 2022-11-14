### Course App

API URLs of course app

|     |     |     |
| --- | --- | --- |
| **Method** | **API URLs** ( URL start with base URL ) | **Operation** |
| GET | /courses | Get all courses |
| GET | /courses/{courseId} | Get single course of given id in URL |
| POST | /courses | Add new course |
| PUT | /courses | Update the course |
| DELETE | /courses/{courseId} | Delete the course |

Follow below steps

URL: Spring Initializer ( https://start.spring.io/ )

Dependencies: Spring Web, MySQL Driver, Spring Data JPA

import project on IDE

in pom.xml set java version which you have based on the declaration while initialising starter project.

application properties

# changing the server code

server.port=9090

#database configuration: mysql

spring.datasource.url=jdbc:mysql://localhost:3306/coursesDB

spring.datasource.username=root

spring.datasource.password=Password@123

spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver

#hibernate configuration

spring.jpa.hibernate.ddl-auto=update

spring.jpa.show-sql=true

spring.jpa.properties.hibernate.dialect = org.hibernate.dialect.MySQL8Dialect

![f670fe8e3254d2996a6fa4ba66c1029e.png](file:///home/shashank/snap/joplin-desktop/28/.config/joplin-desktop/resources/994d7a2f3658460cafd3ea1916d19593.png)

then run below maven command

**./mvnw spring-boot:run**

SQL commands:

mysql -V   // check version

show tables // show all tables in DB

select * from course; // show all course