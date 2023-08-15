# APEX REST Synchronization

Data Synchronization enables developers to automatically sync the contents of a local table with data from a REST service. If the table is not in sync with the Data Profile, Data Synchronization continues to work for columns present in both the table and the Data Profile (other columns are ignored).

You can trigger data synchronization manually or on a regular schedule by using a scheduler job. Note that the CREATE JOB privilege must be granted to the application's parsing schema in order to execute REST source synchronizations on schedule.

Data synchronization use cases:

* provide efficient reporting on large data sets coming from a REST service
* collect data from REST services for consumption by PL/SQL packages or other logic
* collect data from a REST API over a longer period
* use intelligent caching for APEX components

Clearing synchronization settings stops synchronization processing and resets all REST Data Source attributes related to synchronizations. If APEX components are using the local synchronization table, they will be reset to use the REST Service directly.

If no step is defined, the REST Data Source will be invoked once, with default parameters. If steps are defined, APEX will invoke the REST Data Source once for each step, and pass the configured parameters.