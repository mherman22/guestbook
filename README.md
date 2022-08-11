# guestbook
This was done in grails framework.

### What is Grails?
Grails is a web framework based on Groovy and Java which can be deployed into existing Java web servers, e.g., Tomcat or Jetty.

Grails allows to quickly create web applications; its scaffolding capabilities let you create a new project within few minutes. Grails is based on the convention over configuration idea which allows the application to auto-wire itself based on naming schemes (instead of using configuration files, e.g, XML files).

Grails uses JavaEE as the architectural basis and Spring for structuring the application via dependency injection.

The Grails framework allows instance development without requiring any configuration. Just download Grails and you are ready to start. Grails accomplish this by automatically providing the Tomcat web container and the HSQLDB database during development. If you deploy you Grails application later, you can use another web container or database.

Grails is plug-in based and currently uses its own build system (Gant) but plans to migrated to Gradle. The Grails homepage provides several pre-defined plugins which extend the Grails framework.

During the start of a new development with Grails you mainly use the command line to generated new user interfaces.

### Object relationship mapping (ORM) with GORM
Grails uses GORM (Grails Object Relational Mapping) for the persistence of the domain model. GORM is based on Hibernate. You can test with the HSQLDB and run in production against another database simply by changing the configuration file (DataSource.groovy).

### Groovy
![Groovy](https://www.vogella.com/tutorials/Groovy/article.html) is (almost) a superset of Java, e.g., most valid Java constructs are also valid Groovy constructs. Groovy has several advanced features in addition to the standard Java features, e.g., closures, native support for lists and maps, a shorter syntax and much more.

## Installation
- Download the latest official release of Grails from the https://grails.org/download]]Grails download page]. 
- Unzip the download to a directory of your choice.
- Setup your `GRAILS_HOME` environment variable pointing to your installation directory of Grails. Also add the `$GRAILS_HOME/bin` to the PATH variable.
- Please make sure that the environment variable JAVA_HOME is set to the JDK and not the JRE. The JDK is required to develop with Grails.
- Test your installation by opening a command line and running the following command. `grails -version`

### Installing the Grails Eclipse plugin
- The Eclipse IDE has great support for the Grails applications./
Open the Eclipse Update manager via the Help  Install New Software…​menu entry to install the Grails Eclipse plug-in. Enter the following URL in this dialog:
`http://dist.springsource.com/release/TOOLS/update/e4.4/`

### How i created the grails web application above
- Let’s create the application with the name com.vogella.grails.guestbook. #The name of the application is used for the URL on which the application will later run and the WAR file which will be later created.
Create a new directory that will contain your Grails application. Open a command shell, switch to this new directory and type in the following command.
`grails create-app com.vogella.grails.guestbook`.
- After a little while the command line tells you that the application was generated.
This command creates the directory structure and the base configuration of your new web application.

### Run the created application
- The created application can already run. In the shell switch into your directory com.vogella.grails.guestbook. You can then start your application with the following command.
`grails run-app`
- This should start the Grails internal web container and you should receive the message: `server running. Browse to http://localhost:8080/com.vogella.grails.guestbook`
- Open your browser and open the above url.  
- `Congratulations to your first running Grails application!`
