# **RDS (Relational Database Services)**

- RDS is a service which provides database connectivity through the Internet.
- RDS is used to set up, manage and scale a relational database instance in the cloud.
- A database administrator can create, configure, manage and delete an RDS instance, which is a cloud database environment, along with the compute and storage resources it uses.
- RDS adds support for major and minor versions of database engines over time, and an admin can specify an engine version when he or she creates a database instance.
- RDS is Cost-effective,you just pay for what you use, and nothing more. No upfront payment is needed, just the monthly usage payment.
- It just takes a few minutes to scale your infrastructure up or down.
- There are six database engines which RDS provides, and they are:
 1. Amazon Aurora 
 2. PostgreSQL 
 3. MySQL 
 4. MariaDB 
 5. Oracle Database 
 6. Microsoft SQL Server
- Once the database is created and the status is changed to Available you need to connect it with your local MySQL shell and can perform operations.

## steps to Create database

1. step 1: Go to AWS CONSOLE.Then go to services in the menu bar.
2. step 2: select RDS from compute section or you can search for 'rds' in search bar.
3. step 3: Click on 'Create Database'.


![image](https://user-images.githubusercontent.com/63588827/80910103-e3f80500-8d4a-11ea-9dc7-ab1d7306c24e.png)


4. step 4: select methosto create database and whiever search engine you want.


![image](https://user-images.githubusercontent.com/63588827/80910126-0be76880-8d4b-11ea-8863-9573523ab566.png)


5. step 5: keep the default settings for 'database features' and select template as 'free tier'.

6. step 6: in settings,write database identifier name,give id and password for database connetion


![image](https://user-images.githubusercontent.com/63588827/80910385-c035be80-8d4c-11ea-8e3d-902148832f63.png)


7. step 7: keep the default settings for 'db instance size' and 'Availability & durability'.

8. step 8: In 'connectivity' go to advances settings and make db publically accessable.

![image](https://user-images.githubusercontent.com/63588827/80910503-77cad080-8d4d-11ea-83e6-8904654000a9.png)


9. step 9: keep the additional setting default and click on create table.

now you can see your newly created database in the list.


![image](https://user-images.githubusercontent.com/63588827/80910702-f4aa7a00-8d4e-11ea-8d34-95ca31e46bcf.png)

10. you can delete the database by selecting it then click on actions and selete delete to remove the data from the aws cloud.write 'delete me' in the box below.

![image](https://user-images.githubusercontent.com/63588827/80909487-78139d80-8d46-11ea-92f7-88aeacad331f.png)



## Inbound rule settings for port connections
- Go inside your database click on db name lick.
- in connectivity and security click on VPC security groups in security services

![image](https://user-images.githubusercontent.com/63588827/80910868-1c4e1200-8d50-11ea-93b5-b626c98ec959.png)


- click on inbound rule in the menu below.
- click edit inbound rule

![image](https://user-images.githubusercontent.com/63588827/80910901-54edeb80-8d50-11ea-9bf0-3fd542eb2c34.png)

- click on 'add rule'
- give port range as 3306 and source as 'anywhere'.and then click on save rules.now you can see port setting like this.


![image](https://user-images.githubusercontent.com/63588827/80910952-c6c63500-8d50-11ea-92c7-ccb46fbd91ae.png)


## operating database through mysql workbench

- open Mysql workbench.
- click on '+' in Mysqlconnection' to make new connection

![image](https://user-images.githubusercontent.com/63588827/80911007-2290be00-8d51-11ea-92b4-11c2241350d4.png)


- give  new name to the connection.
- select hostname as your rds endpoint detail
- give username and password as you provided at the time of creation.
- and the click on 'test connection'.

![image](https://user-images.githubusercontent.com/63588827/80911074-84512800-8d51-11ea-9865-b21421a2648e.png)


- when connection is successful then click on ok.
- now you successfully created the connection 

![image](https://user-images.githubusercontent.com/63588827/80911123-00e40680-8d52-11ea-8d9b-1d780b97e899.png)

- now double click on new connection you have just made.
- you will see the some already given databases by the aws services.
- now you can do any operatio the rds you have made.

![image](https://user-images.githubusercontent.com/63588827/80911186-6e903280-8d52-11ea-8703-5479255b616c.png)

![image](https://user-images.githubusercontent.com/63588827/80911074-84512800-8d51-11ea-9865-b21421a2648e.png)



