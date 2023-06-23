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

