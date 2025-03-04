# My Maven Tomcat Application

This project is a simple web application that demonstrates how to create a "Hello World" website using Maven and deploy it on Apache Tomcat.

## Project Structure

```
my-maven-tomcat-app
├── src
│   ├── main
│   │   ├── java
│   │   │   └── com
│   │   │       └── example
│   │   │           └── HelloWorldServlet.java
│   │   ├── resources
│   │   └── webapp
│   │       ├── WEB-INF
│   │       │   └── web.xml
│   │       └── index.jsp
│   └── test
│       └── java
│           └── com
│               └── example
│                   └── HelloWorldServletTest.java
├── pom.xml
└── README.md
```

## Prerequisites

- Java Development Kit (JDK) 8 or higher
- Apache Maven
- Apache Tomcat

## Building the Project

To build the project, navigate to the project directory and run the following command:

```
mvn clean package
```

This will compile the Java code, run tests, and package the application into a WAR file located in the `target` directory.

## Running the Application

1. Deploy the generated WAR file (located in `target/my-maven-tomcat-app.war`) to your Apache Tomcat server. You can do this by copying the WAR file to the `webapps` directory of your Tomcat installation.
2. Start the Tomcat server.
3. Access the application in your web browser at the following URL:

```
http://localhost:8080/my-maven-tomcat-app/
```

You should see "Hello, World!" displayed on the page.

## Testing

To run the unit tests, execute the following command:

```
mvn test
```

This will run the tests defined in `HelloWorldServletTest.java` to ensure that the `HelloWorldServlet` behaves as expected.

## License

This project is licensed under the MIT License. See the LICENSE file for more details.