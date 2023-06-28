# APEX REST Data Sources

REST Data Sources enables developers to access REST services, or generic JSON data feeds in applications and use the data in APEX components such as reports, interactive reports, and interactive grids.

A REST data source can contain one or many operations which are the references to a concrete external web service.

REST data sources contain multiple operators that differ depending on the web service target. For a REST service, an operation is a specific service handler (such as GET, PUT, POST, or DELETE).

Oracle APEX splits the endpoint URL of a web service into two parts. The server-specific part is stored as a separate entity called the **Remote Server**. You can reuse a remote server with multiple REST data sources if it uses the same server, or an URL path prefix, or context route. 