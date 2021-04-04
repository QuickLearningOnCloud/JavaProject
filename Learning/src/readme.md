Download JDBC driver for MySQL
First, in order to have Java program working with MySQL, we need a JDBC driver for MySQL. Browse this URL:
http://dev.mysql.com/downloads/connector/j/
to download the latest version of the JDBC driver for MySQL called Connector/J. MySQL Connector/J comes into 2 major versions: 5.1 and 8.0. The latest version 8.0 supports JDBC 4.2 and JDK 8 or higher.
download jdbc driver for mysql



No need to load MySQL driver class explicitly
The Connector/J version 8.0 library comes with a JDBC driver class: com.mysql.cj.jdbc.Driver. Before Java 6, we have to load the driver explicitly by this statement:
Class.forName("com.mysql.cj.jdbc.Driver");

However that statement is no longer needed, thanks to new update in JDBC 4.0 comes from Java 6. As long as you put the MySQL JDBC driver JAR file  file into your program’s classpath, the driver manager can find and load the driver.