## Prerequisites
- Eclipse
- java 17
- Create the starting project using https://start.spring.io/
- Spring Boot 3+ works only with Java 17+

## Running Examples
- Download the zip or clone the Git repository.
- Unzip the zip file (if you downloaded one)
- Open Command Prompt and Change directory (cd) to folder containing pom.xml
- Open Eclipse 
   - File -> Import -> Existing Maven Project -> Navigate to the folder where you unzipped the zip
   - Select the right project
- Choose the Spring Boot Application file (search for @SpringBootApplication)
- Right Click on the file and Run as Java Application
- You are all Set
- For help : use our installation guide - https://www.youtube.com/playlist?list=PLBBog2r6uMCSmMVTW_QmDLyASBvovyAO3

 ## Configure H2 in-memory database
  - http://localhost:8080/h2-console
  - Use db url jdbc:h2:mem:testdb
 
 ## Launch MySQL using Docker
  - Open the docker desktop
  - run this below command from cmd
  - port to see my-sql: jdbc:mysql://localhost:3306/todos

```
docker run --detach --env MYSQL_ROOT_PASSWORD=dummypassword --env MYSQL_USER=todos-user --env MYSQL_PASSWORD=dummytodos --env MYSQL_DATABASE=todos --name mysql --publish 3306:3306 mysql:8-oracle
```
