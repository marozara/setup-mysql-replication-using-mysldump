# **How to setup mysql replication using mysqldump ?**
## Using mysqldump we have two scenarios in which we can setup a MySQL replication.
- Scenario 1 : dump database from primary instance
- Scenario 2 : dump database from replica instance
### Now let's explore these two scenarios.
### 1. Scenario One (dump database from primary instance)
Usually, we setup replication using the primary instance if there is no replication yet in place for the instance or 

> myqldump -u username -p  --master-data dabase_name  > database_name.sql

### 2. Scenario two (dump database from replica instance)

> mysqldump -u username -p --dump-slave database_name > database_name.sql 
