# :oncoming_taxi: Simple Taxi Service :oncoming_taxi:
[![forthebadge](https://forthebadge.com/images/badges/made-with-java.svg)](https://forthebadge.com)
# About the application

That's a simple taxi web application, which can work with basic CRUD operations.
# Structure of the project

Application has basic structure with adherence to all SOLID principles and N-tier architecture :
* The package `controller` has all the controllers needed to work with basic CRUD operations through HTTP.
* The package `dao` has all services and implementatiosn for accessing data from DB.
* The package `exception` has two costum exceptions which are used in the application. 
* The package `lib` contains `Injector` to uphold the principle of *Dependency injection* and all needed annotations.
* The package `model` contains `Driver` model, which behave as User and models of `Car` and `Manufacturer`.
* The package `service` is responsible for working with the DAO and does not allow working with the DB at the controller level.
* The package `util` has `ConnectionUtil` for making a connection with your DB.
* The package `web.filter` has `AuthenticationFilter`: that an object that is invoked at the preprocessing and postprocessing of a request.
* The directory `resources` has a `init_db.sql` file, that should be used to properly structure the database.
* The directory `webapp` contains all needed JSPs for displaying an application in browser and the package `css` with primitive styles for an app.

# Used technologies
* **JAVA**
* **HTML**
* **CSS**
* **SQL**

# Installation
1. IntelliJ IDEA <sub> [download link](https://www.jetbrains.com/idea/download/#section=windows) </sub>, JDK<sub> [download link](https://www.oracle.com/cis/java/technologies/javase/jdk11-archive-downloads.html) </sub> should be installed on your PC

2. Install GIT <sub> [download link](https://git-scm.com/downloads) </sub> and setup it <sub> [setup instruction](https://githowto.com/setup)

3. Install Apache Maven <sub> [download link](https://maven.apache.org/install.html) </sub> and add `PATH` variables <sub> [adding variables instruction](https://stackoverflow.com/questions/45119595/how-to-add-maven-to-the-path-variable) </sub>

4. Install MySQL <sub> [download link](https://dev.mysql.com/downloads/installer/) </sub> and setup it <sub> [video guide](https://www.youtube.com/watch?v=6MvJsqloIco) </sub>

5. Setup your SSH key <sub> [GIThub guide](https://docs.github.com/ru/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account) </sub>

6. Now you need to fork project to your repo, you can do it by clicking ![image](https://user-images.githubusercontent.com/118058456/227191760-e5238095-4b06-4076-ba0e-464717de2fcb.png)

7. Go to IntelliJ IDEA and create new project from Version Control  ![image](https://user-images.githubusercontent.com/118058456/227191922-30c60041-3181-470b-9ca9-e53e4aef7eaf.png)

8. From your recently made repository click Code button, choose SSH and paste the link into IntelliJ IDEA ![image](https://user-images.githubusercontent.com/118058456/227192265-c8d209e6-1ad6-4ac0-8827-1649eabd7c2a.png)

9. Now change parameters in `ConnectionUtil` for connecting to DB.

10. Install Apache Tomcat <sub> [download link](https://tomcat.apache.org/download-90.cgi) </sub>, add configuration for your project here ![image](https://user-images.githubusercontent.com/118058456/227192947-02e1e248-78d0-4085-a748-1ca2804f2409.png)

11. Run the project and check the result ! :see_no_evil:

