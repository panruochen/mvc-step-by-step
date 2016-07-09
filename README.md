## MVC Step by Step

This projoct is based on MVC-step-by-step tutorials which could be found in spring-mvc docs.   </br>
It has fixed the compile or runtime errors which are introduced from the original tutorials by mistake.

### Runtime Environment
- Windows 7
- Tomecat   </br>
  http://tomcat.apache.org/download-60.cgi
- Spring-framework-2.5   </br>
  https://sourceforge.net/projects/springframework/files/springframework-2/2.5/spring-framework-2.5-with-dependencies.zip/download
- Java7/8 with JAVE\_HOME env variable set
- Ant

### Installation Path
Tomcat is assumed to be installed in C:\mvc-step-by-step\apache-tomcat-6.0.45  </br>
springapp in C:\mvc-step-by-step\springapp  </br>
In the following part of this README, %TOMCAT% and %SPRINGAPP% refer to the installation directories respectively.

### Run this example
1. Conigure Tomcat
   Add the following two lines into %TOMCAT%\conf\tomcat-users.xml   </br>
```
   <role rolename="manager"/>
   <user username="tomcat" password="s3cret" roles="manager"/>
```

2. Deploy this Web Application (springapp) to Tomcat
   </br>
```
ant deploy
```
  </br>
  If your Tomcat is not in the assumed directory, please fix it in %SPRINGAPP%\build.properties

3. Start Database server
   </br>
```
cd %TOMCAT%\db
server.bat
```

4. Create a database
   </br>
```
ant dbTests
```

5. Start Apache Http Server
   </br>
```
%TOMCAT%\bin\startup.bat
```

6. Visit the following link in the browser
   </br>
```
http://localhost:8080/springapp/
```
