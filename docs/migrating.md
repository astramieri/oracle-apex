# Migrating Applications 

An APEX application can readily be moved from one environment to another. It is a normal practice to move an application from development to test and into production. This generally involves exporting the application from development and importing it into test or production environment.

Along with the application definition, you also need to export the underlying database objects and the seed data. So you need to create the DDL as well as the DML scripts.

**NOTE**: You cannot import an APEX application into an earlier release of APEX. 

