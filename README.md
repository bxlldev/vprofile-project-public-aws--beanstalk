# Prerequisites
#
- JDK 11 
- Maven 3 
- MySQL 8

# AWS Services & Techstacks:
![image](https://github.com/bxlldev/vprofile-project-public-aws--beanstalk/assets/127035655/62543707-4df5-4e39-895d-043037bd30fb)

- Beanstalk			    <=>		Tomcat EC2/VM
- ELB in Beanstalk	<=>		Nginx LB/ELB
- Autoscaling			  <=>		None /Autoscaling
- EFS/S3			  	  <=>		NFS /S3/EFS
- RDS				    	  <=>		MySQL on VM/EC2
- Elastic Cache		  <=>		Memcached on VM/EC2
- Active MQ			    <=>		RabbitMQ on VM/EC2
- Route53				    <=>		GoDaddy, local DNS
- CloudFront		   	<=>		None /Multi DC Across the world
  
# Database
Here,we used Mysql DB 
sql dump file:
- /src/main/resources/db_backup.sql
- db_backup.sql file is a mysql dump file.we have to import this dump to mysql db server
- > mysql -u <user_name> -p accounts < db_backup.sql


