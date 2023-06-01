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

### 💡 TECHNOLOGIES 💡
> - Maven version 3.8.0
> - Java version 17.0.2
> - Tomcat version 9.0.73
> - MySQL version 8.0.22
> - Java Servlets version 4.0.1
> - JDBC version 4.2
> - JSTL version 1.2

### 🚀 STRUCTURE 🚀

__Controller:__
   - Authentication controllers:
      - LoginController - to login
      - LogoutController - to logout
   - Car controllers:
      - AddCarController - to create new car 
      - AddDriverToCarController - to add driver to the car
      - DeleteCarController - to delete car
      - GetAllCarsController - to display all cars
   - Driver controllers:
      - AddDriverController - to register driver
      - DeleteDriverController - to delete driver
      - GetAllDriversController - to display all drivers
      - GetMyCurrentCarsController - to display cars on current account
   - Manufacturer controllers:
      - AddManufacturerController - to add new manufacturer
      - DeleteManufacturerController - to delete manufacturer
      - GetAllManufacturersController - to display all manufacturers
   - IndexController - homepage
__Dao:__
   - CarDaoImpl - processes car model from DB
   - DriverDaoImpl - processes driver model from DB
   - ManufacturerDaoImpl - processes manufacturer model from DB
__Exception:__
   - AuthenticationException 
   - DataProcessingException
__Model:__
   - Car - car model class
   - Driver - driver model class
   - Manufacturer - manufacturer model class
__Service:__
   - AuthenticationServiceImpl - processes authentication logic
   - CarServiceImpl - processes car's CRUD logic
   - DriverServiceImpl - processes driver's CRUD logic
   - ManufacturerServiceImpl - processes manufacturer's CRUD logic
__Util:__
   - ConnectionUtil - provides a connection to the database
__Resources:__
   - init_db.sql - sql script to initialize the database
__Webapp:__
   - jsp files
   - css file 
   - web.xml - configuration file

### 🔍 GETTING STARTED 🔍
> - Clone the project repository.
> - Execute the SQL script located in src/main/resources/init_db.sql to initialize the database.
> - Update the values of `URL`, `USERNAME`, `PASSWORD` and `JDBC_DRIVER` in the src/main/java/util/ConnectionUtil file with your own database configuration.
> - Build the project using Maven: `mvn clean install`.
> - Deploy the generated WAR file to your servlet container. (This project uses Tomcat.)
> - After deploying the project, open the following 
[http://localhost:8080](http://localhost:8080) <br> in your web browser to access the taxi service.
