# TAXI-SERVICE
 
 <p align="center">
  <img src="https://github.com/SofiiaKazanivska/TAXI-SERVICE/blob/main/taxi_service.jpg" alt="Taxi Service" width="400">
</p>


This project serves as an educational platform that showcases the functionality of a taxi service. Users have the ability to perform various actions such as adding new drivers, registering new cars within the service, including information about car manufacturers, assigning drivers to specific vehicles, and accessing comprehensive details about drivers, cars, and manufacturers. The project incorporates user-friendly navigation between different pages to enhance the overall user experience.

### ⭐️ FEATURES ⭐️
> - Authentication
> - Display current cars
> - Display all drivers
> - Display all cars
> - Display all manufacturers
> - Add driver to car
> - Add new driver
> - Add new car
> - Add new manufacturer


### 🚀 STRUCTURE 🚀

__Controller:__

  > - *Authentication controllers:*
  >   - LoginController - to login
  >   - LogoutController - to logout
  > - *Car controllers:*
  >   - AddCarController - to create new car 
  >   - AddDriverToCarController - to add driver to the car
  >    - DeleteCarController - to delete car
  >    - GetAllCarsController - to display all cars
  > - *Driver controllers:*
  >    - AddDriverController - to register driver
  >    - DeleteDriverController - to delete driver
  >    - GetAllDriversController - to display all drivers
  >    - GetMyCurrentCarsController - to display cars on current account
  > - *Manufacturer controllers:*
  >    - AddManufacturerController - to add new manufacturer
  >    - DeleteManufacturerController - to delete manufacturer
  >    - GetAllManufacturersController - to display all manufacturers
  > - *IndexController:*
  >    - homepage
    
__Dao:__
  > - CarDaoImpl - processes car model from DB
  > - DriverDaoImpl - processes driver model from DB
  > - ManufacturerDaoImpl - processes manufacturer model from DB

__Exception:__
 >  - AuthenticationException 
 >  - DataProcessingException

__Model:__
  > - Car - car model class
  > - Driver - driver model class
  > - Manufacturer - manufacturer model class
   
__Service:__
  > - AuthenticationServiceImpl - processes authentication logic
  > - CarServiceImpl - processes car's CRUD logic
  > - DriverServiceImpl - processes driver's CRUD logic
  > - ManufacturerServiceImpl - processes manufacturer's CRUD logic

__Util:__
  > - ConnectionUtil - provides a connection to the database

__Resources:__
  > - init_db.sql - sql script to initialize the database

__Webapp:__
  > - jsp files
  > - css file 
  > - web.xml - configuration file

### 🔍 GETTING STARTED 🔍
> - Clone the project repository.
> - Execute the SQL script located in src/main/resources/init_db.sql to initialize the database.
> - Update the values of `URL`, `USERNAME`, `PASSWORD` and `JDBC_DRIVER` in the src/main/java/util/ConnectionUtil file with your own database configuration.
> - Build the project using Maven: `mvn clean install`.
> - Deploy the generated WAR file to your servlet container. (This project uses Tomcat.)
> - After deploying the project, open the following 
[http://localhost:8080](http://localhost:8080) <br> in your web browser to access the taxi service.



### 💡 TECHNOLOGIES 💡
> - **Maven** `v.3.10.1` - build tool and dependency management
> - **JDK** `v.17.0.2` - Java Development Kit
> - **MySql** `v.8.0.22` - relational database management system
> - **Tomcat** `v.9.0.73` - server for deploying Java web applications
> - **Java Servlets** `v.4.0.1` - a technology for developing web applications in Java
> - **JDBC** `v.4.2` - Java Database Connectivity
> - **JSTL** `v.1.2` - JavaServer Pages Standard Tag Library


 <a href="https://mvnrepository.com/artifact/org.apache.maven.plugins/maven-compiler-plugin/3.10.1">
    <img src="https://maven.apache.org/images/maven-logo-black-on-white.png" alt="Maven" width="50" height="25">
</a>


  [![JDK](https://img.shields.io/badge/JDK-v.17.0.2-orange)](https://www.oracle.com/java/technologies/javase-jdk17-downloads.html)


   [![MySQL](https://img.shields.io/badge/MySQL-v.8.0.22-blue)](https://dev.mysql.com/downloads/mysql/8.0.22.html)


   [![Tomcat](https://img.shields.io/badge/Tomcat-v.9.0.73-yellowgreen)](https://tomcat.apache.org/download-90.cgi)


   [![Java Servlets API](https://img.shields.io/badge/Java%20Servlets%20API-v.4.0.1-blueviolet)](https://mvnrepository.com/artifact/javax.servlet/javax.servlet-api/4.0.1)

   [![JDBC](https://img.shields.io/badge/JDBC-v.4.2-lightgrey)](https://mvnrepository.com/artifact/org.apache.maven.plugins/maven-compiler-plugin/3.10.1)

   [![JSTL](https://img.shields.io/badge/JSTL-v.1.2-yellow)](https://mvnrepository.com/artifact/javax.servlet/jstl/1.2)


### 💬 Contact 💬
	
[Kazanivska Sofiia](https://www.linkedin.com/in/sofiia-kazanivska-40a413232/) <br>
sofiakazzz@gmail.com
