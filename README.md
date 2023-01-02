# Dev_website_signup_java.
Download eclipse and tomcat server, Add tomcat server to eclipse.
Try help from internet if not able to configure eclipse tomcat server.
Create dynamic web project in eclipse and give any name("signup_web")
Extract downloaded Zip file and copy the content inside Dev_website_signup_java folder and pase it to signup_web folder.
Before pasting delete all the default folders inside signup_web folder.
Now go to this path "Dev_website_signup_java-master\src\main\webapp\WEB-INF\lib".
copy "mysql-connector-java-8.0.13" and paste in inside tomcat "lib" folder ("C:\Program Files\Apache Software Foundation\Tomcat 10.0\lib")
install Mysql create new Schemas named signup_project then:
Below command must be used:

use signup_project;
create table users
(
	id int primary key auto_increment,
    uname varchar(50),
    upwd varchar(50),
    uemail varchar(50),
    umobile varchar(20)
    );

now table is created.

Now go to path "signup_web\src\main\java in eclips open RegistrationServelet.java,
In line number(60) "con = DriverManager.getConnection("jdbc:mysql://localhost:3306/signup_project?useSSL=false","root","Devsingh5@");"
in place of "root" and "Devsingh5@" give you username and password of mysql;

now Right click on signup_web folder and click run on server now done.
