# Migrating Applications 

An APEX application can readily be moved from one environment to another. It is a normal practice to move an application from development to test and into production. This generally involves exporting the application from development and importing it into test or production environment.

Along with the application definition, you also need to export the underlying database objects and the seed data. So you need to create the DDL as well as the DML scripts.

**NOTE**: You cannot import an APEX application into an earlier release of APEX. 

As you define applications, pages, regions, items, and so forth, the definitions are saved in various tables defined within the APEX engine schema. When you export an application, a single SQL file is created by extracting the application definitions from the metadata tables. When importing the applications, records are inserted or updated if overwriting an existing application into the APEX metadata tables. Therefore, once an application is imported, all the application definitions can be reviewed from the Application Builder, and the application can be run immediately.

## One-click Remote Application Deployment Wizard

Using a simple wizard, you can now directly export and deploy your application along with the supporting objects into the target system.

From within your development environment, you can deploy your application to the remote production environment. You do not need to directly access your production environment to import this application.

One-click remote application deployment is authenticated through:

- first party authentication (Basic Authentication)
- schema authentication (database username and password)
- OAuth 2 Client Credentials.