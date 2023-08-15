# APEX REST Enabled SQL Reference

Developers create REST enabled SQL service references to execute SQL or PL/SQL defined on a remote Oracle database.

Developers create REST enabled SQL references by defining a name, the endpoint URL, and authentication information within shared components. 

REST enabled SQL references requirements:

- set up a remote Oracle database

- install Oracle REST Data Services(ORDS) 19.x or later
	
	*(this ORDS installation is completely independent of the Oracle REST Data Services used as APEX web server)*

- configure and enable the REST enabled SQL service feature

- ativate REST enabled SQL services for the target schema on the remote database to be accessed by running or **ORDS.ENABLE_SCHEMA**

The REST enabled SQL service is available with a URL in the following format 

	http://host:port/ords/schema

## Differences between REST Enabled SQL Service References and Database Links

1. Functions at the workspace-level. Developers can create an APEX component with a query on a REST enabled SQL Service but cannot join it to a local table.
2. Works with JSON over HTTP(s) which makes it easy-to-use it in Cloud environments or over the internet.

## Exporting and Importing REST Enabled SQL Services

When you export an application, used REST Enabled SQL references are added to the export file. If you export an application and import it into another workspace, APEX checks whether the target workspace already contains REST Enabled SQL references with the same static ID. If a REST Enabled SQL reference already exists, the application uses the existing reference. If the reference does not exist, it is created in the target workspace.

## Links

[Oracle REST Data Services Quick Start Guide](https://docs.oracle.com/en/database/oracle/oracle-rest-data-services/23.1/qsord/get-started-with-oracle-rest-data-services.html#GUID-0CE142F6-2252-4099-ADF4-BD61FACAFF9D)

[Enabling REST services for Autonomous Database](https://cloudness.net/enable-ords-oracle-autonomous-database/)

