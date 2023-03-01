### Describe the Azure SQL family of products including Azure SQL Database, Azure SQL
1. **SQL Server on Azure Virtual Machines**  
IaaS service where a virtual machine is provisioned for you with SQL Server pre-installed. Can easily migrate from on-premises SQL Server setups. Since it's IAAS, the consumer will be responsible for updating and maintaining the virtual machine and database.  

2. **Azure SQL Managed Instance**  
PaaS service where some general tasks are abstracted from the user, such as backups and database monitoring, but you are still responsible for security and resource allocation of your databases. Almost fully compatible with on-premises instances of SQL Server and can be used for data migrations. Also offers services like Service Brokers or Database Mail that isn't available on the other services.  

3. **Azure SQL Database**  
Fully managed PaaS service. Available in two forms: 
- Single Database: Create and run your database on an isolated server. With the serverless configuration, Microsoft creates the database server which you may share with other databases (but the privacy of your database remains).  
- Elastic Pool: Your databases are pooled and access the same computing resources such as memory, space, and processing power. Can help cut costs.  

### Managed Instance, and SQL Server on Azure Virtual Machines
• Identify Azure database services for open-source database systems`**S