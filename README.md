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

### Conigure Tomcat
   Add the following two lines into %TOMCAT%\conf\tomcat-users.xml   </br>
```
   <role rolename="manager"/>
   <user username="tomcat" password="s3cret" roles="manager"/>
```

### Start/Stop Apache Http Server
Start: %TOMCAT%\bin\startup.bat    </br>
Stop:  %TOMCAT%\bin\shutdown.bat   </br>


