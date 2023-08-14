# APEX REST Synchronization

Data Synchronization enables developers to automatically sync the contents of a local table with data from a REST service. You can trigger data synchronization manually or on a regular schedule by using a scheduler job. 

    Note that the CREATE JOB privilege must be granted to the application's parsing schema in order to execute REST source synchronizations on schedule.

Data synchronization use cases:
* provide efficient reporting on large data sets coming from a REST service
* collect data from REST services for consumption by PL/SQL packages or other logic
* collect data from a REST API over a longer period
* use intelligent caching for APEX components