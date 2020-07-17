# ZipToDest


## Maven Modules
 ZD-Client - Contains angular code
 ZD-Server - Contains API to support UI related to oracle database
 ZD-Iseries - Contains API to support UI related to Iseries only.
 ZD-Distribution - Contains API for distribution from master table. 

## Build
go to ZipToDest-UI>
Run mvn clean install -DskipITs -DskipTests  

## Running unit tests
go to ZipToDest-UI>
Run mvn clean test

## Bringing up UI
go to ZipToDest-UI\ZD-Server>
mvn spring-boot:run -Dspring.profiles.active=lcl (for running with in memory database)
mvn spring-boot:run -Dspring.profiles.active=dev (for running with oracle database


## Bringing up Distribution API
go to ZipToDest-UI\ZD-Distribution>
mvn spring-boot:run -Dspring.profiles.active=lcl (for running with in memory database)
mvn spring-boot:run -Dspring.profiles.active=dev (for running with oracle database

